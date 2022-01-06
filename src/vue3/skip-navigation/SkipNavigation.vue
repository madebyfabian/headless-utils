<template>
	<div
		class="SkipNavigation"
		ref="skipTo"
		:data-is-focused="isFocused"
	>
		<SkipNavigationElement
			@focused="focusWithin"
			@focus-within="focusWithin"
			v-bind="props"
		/>
	</div>
</template>

<script>
import SkipNavigationElement from './SkipNavigationElement.vue'
import { programmaticFocus } from './util'
export default {
  name: 'SkipNavigation',
	components: {
		SkipNavigationElement
	},
  props: {
    listLabel: {
      type: String,
      default: 'Skip to'
    },
    label: {
      type: String,
      default: 'Skip to main content'
    },
    to: {
      type: String,
      default: '#main'
    }
  },
  data () {
    return {
      isFocused: false
    }
  },
  mounted () {
    if (this.$route) {
      this.$watch('$route.path', () => {
        this.$nextTick(() => programmaticFocus(this.$refs.skipTo))
      })
    }
  },
  computed: {
    props () {
      return { label: this.label, to: this.to }
    }
  },
  methods: {
    focusWithin (val) {
      this.isFocused = val
    }
  }
}
</script>
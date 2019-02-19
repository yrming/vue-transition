<script>
export default {
    name: 'vue-transition',
    functional: true,
    render (h, context) {
        return h('transition', context.data, context.children);
    }
};
</script>
<style>
    .fade-enter, .fade-leave-to {
        opacity: 0.01;
    }
    .fade-enter-active {
        transition: opacity 300ms cubic-bezier(0.215, 0.61, 0.355, 1)
    }
    .fade-leave-active {
        transition: opacity 250ms linear;
    }
</style>
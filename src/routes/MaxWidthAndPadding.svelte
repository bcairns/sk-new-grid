<script>
    let _class = '';
    export { _class as class };
</script>

<div class="lg:max-w-[1010px] px-4 md:px-8 mx-auto {_class}">
    <slot />
</div>

<style>
    @media (min-width: 1080px) {
        div {
            max-width: 1560px;
            padding-left: 60px;
            padding-right: 60px;
        }
    }
</style>
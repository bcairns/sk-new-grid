<script>
    import MaxWidthAndPadding from "./MaxWidthAndPadding.svelte";
    import Box from "./Box.svelte";
    import TextContainer from "./TextContainer.svelte";
</script>

<MaxWidthAndPadding class="grid gap grid-cols-2 md:grid-cols-3 my-16">
    <Box />
    <Box />
    <Box />
    <Box />
    <Box />
    <Box />
</MaxWidthAndPadding>

<MaxWidthAndPadding class="my-16">
    <h2 class="font-bold">Excessive Line-Length</h2>

    <p>Call it "The Privacy Page Problem" - Simple pages with single-column text can quickly grow unreadable, our current pages like this at 1200px are already way past good readability (<a target="_blank" href="https://www.logitech.com/en-us/tos/terms.html">example</a>). If we are increasing the "standard max width" from 1200px to 1440px, we should account for this.  Text containers should have a max width ideally between 45 - 80 characters (which should <em>never</em> need to be set by authors; eg specifying "padding columns").</p>


    <p>
        Aliquam erat volutpat. Suspendisse potenti. Donec ac finibus risus. Morbi nec enim velit. Nam nec risus at elit placerat lacinia a id dolor. Nam laoreet mauris quis risus fermentum, a consectetur mauris pulvinar. Cras blandit scelerisque eros nec tempor. Integer nibh arcu, euismod eu rhoncus id, elementum eget diam. Nullam volutpat imperdiet purus. Duis quis nibh dignissim, facilisis sapien id, facilisis elit.
    </p>

    <TextContainer>
        <h2 class="font-bold pt-8">Better Line-Length (~80ch)</h2>

        <p class="">
            Curabitur fringilla, ante id faucibus euismod, tortor eros congue odio, eu feugiat neque magna in nibh. Vivamus consectetur auctor augue, vel eleifend quam aliquet vel. Vestibulum nec ante nibh. Vivamus ultrices ex quis neque venenatis ornare. Vivamus ac dui vehicula, tincidunt sapien sit amet, ultricies diam. Aenean iaculis urna blandit nulla maximus finibus. Vestibulum tincidunt aliquet purus ac lobortis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Aliquam erat volutpat. Vivamus at porta ex, eu egestas massa. Suspendisse eget dui turpis.
        </p>
        <p>
            In cursus felis vitae pretium tincidunt. Phasellus mollis dolor et nisi convallis, id mollis felis iaculis. Praesent tincidunt elit justo, ut varius elit consectetur vitae. Praesent eu consectetur libero, et tempus tortor. Donec ac nulla a turpis fringilla feugiat. Pellentesque malesuada arcu enim, nec cursus neque congue quis. Nulla facilisi. Integer a urna in libero faucibus mattis sed at lacus.
        </p>
    </TextContainer>
</MaxWidthAndPadding>

<style lang="scss">
    p {
        @apply my-3;
    }
    a {
        color: blue;
      &:hover {
        @apply underline;
      }
    }
</style>
<template>
    <div>
        <slot></slot>
    </div>

</template>

<script>
    import Flickity from 'flickity'
    import 'flickity/dist/flickity.min.css'
    import 'flickity-bg-lazyload'

    export default {
        props: {
            wraparound: { default: true},
            autoplay: { default: false},
            prevnextbuttons: { default: false},

        },

        mounted() {
            // console.log(this.$el)
            new Flickity(this.$el, {
                wrapAround: this.wraparound,
                autoPlay: this.autoplay,
                prevNextButtons: this.prevnextbuttons,

                bgLazyLoad: true,
                pageDots: false,
                setGallerySize: true
            }).focus()
        }
    }

</script>

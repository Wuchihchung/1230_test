<template>
    <div class="imageWrapper" ref="imageWrapper">
        <img class="real_pic" :src="dataURL" />
        <slot></slot>
    </div>
</template>

<script>
export default {
    data() {
        return {
            dataURL: ''
        }
    },
    methods: {
        toImage() {
            html2canvas(this.$refs.imageWrapper,{
                backgroundColor: null
            }).then((canvas) => {
                let dataURL = canvas.toDataURL("image/png");
                this.dataURL = dataURL;
            });
        }
    }
}
</script>
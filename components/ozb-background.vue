<template>
    <div>
        <img class="background__bridge" src="~/assets/img/open-zaakbrug-brug.svg" />
        <div class="background"></div>
    </div>
</template>
  
<script>
export default {
    name: 'Background',

    mounted() {
        this.animateBg();
    },

    methods: {
        animateBg() {
            this.$gsap.to('.background', {
                duration: .3,
                ease: 'Power1.easeInOut',
                '--bg-rotation': `220deg`,
                '--bg-fade-color': `rgba(255, 0, 61, .36)`,
                scrollTrigger: {
                    start: '+=600',
                    toggleActions: "play none none reverse",
                }
            })
            this.$gsap.to('.background__bridge', {
                duration: .3,
                ease: 'Power1.easeInOut',
                opacity: 0,
                scrollTrigger: {
                    start: '+=600',
                    toggleActions: "play none none reverse",
                }
            })
        }
    }
}
</script>
  
<style scoped>
:root {
    --bg-rotation: 140deg;
    --bg-fade-color: rgba(0, 255, 194, .36);
}

.background {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    z-index: -1;
    background: linear-gradient(var(--bg-rotation), var(--bg-fade-color) 0%, rgba(255, 255, 255, 0) 50%);
}

.background__bridge {
    z-index: -2;
    max-width: 50vw;
    bottom: -20px;
    position: fixed;
    right: 20px;
    opacity: 0.2;
}
</style>
  
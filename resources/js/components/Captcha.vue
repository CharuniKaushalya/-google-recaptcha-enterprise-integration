<template>
    <div>
        <div id="g-recaptcha"></div>
    </div>
</template>

<script>
export default {
    mounted() {
        grecaptcha.enterprise.render('g-recaptcha', {
            'sitekey' : '6LcaPDgeAAAAAPvMCsGRx1PVL3n1XOR9RK8kDnek',
        });
    },
}
</script>

<style scoped>

</style>

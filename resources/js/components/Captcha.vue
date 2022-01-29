<template>
    <div>
        <div id="g-recaptcha"></div>
    </div>
</template>

<script>
export default {

    mounted() {
        var vueRecaptchaApiLoaded = function() {
            grecaptcha.enterprise.render('g-recaptcha', {
                'sitekey' : '6LcaPDgeAAAAAPvMCsGRx1PVL3n1XOR9RK8kDnek'
            });
        };

        window.vueRecaptchaApiLoaded =  vueRecaptchaApiLoaded

        // const script = document.createElement('script')
        // script.id = 'recaptchascrpitid'
        // script.src = `https://www.google.com/recaptcha/enterprise.js?onload=vueRecaptchaApiLoaded&render=explicit`
        // script.async = true
        // script.defer = true
        //
        // document.head.appendChild(script)
    },
}
</script>

<style scoped>

</style>

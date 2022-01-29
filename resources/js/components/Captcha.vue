<template>
    <div>
        <div id="g-recaptcha"></div>
    </div>
</template>

<script>
export default {
    // data() {
    //     dd:Object.prototype.hasOwnProperty.call(window, 'grecaptcha')
    // },
    //
    // // computed : {
    // //     dd() {
    // //         return
    // //     }
    // // },
    //
    // watch: {
    //   dd() {
    //       console.log("here come 222")
    //   }
    // },

    mounted() {
        var vueRecaptchaApiLoaded = function() {
            grecaptcha.enterprise.render('g-recaptcha', {
                'sitekey' : process.env.MIX_RECAPTCHA_SITE_KEY
            });
        };

        window.vueRecaptchaApiLoaded =  vueRecaptchaApiLoaded
        //
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

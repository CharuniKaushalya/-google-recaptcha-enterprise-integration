<template>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-md-8">
                <div class="card">
                    <div class="card-header">Home</div>

                    <div class="card-body">
                        <captcha></captcha>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import Captcha from './Captcha.vue'

export default {
    components: { Captcha },

    mounted() {
        console.log('Component mounted.')
    }
}
</script>

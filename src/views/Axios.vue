<template>123123</template>

<script lang="ts">
import { defineComponent } from 'vue'
import axios from '@/utils/axios'

export default {
    name: 'Axios',
    setup() {
        axios
            .get('/user/XPoet')
            .then((res) => {
                console.log('res', res)
            })
            .catch((err) => {
                console.log('err', err)
            })
    }
}
</script>

<style lang="stylus" scoped></style>

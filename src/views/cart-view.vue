<template>
    <cartComp v-show="showModal" @close-modal="showModal = false"/>
    <div class="save-btn">
    <button @click="showModal = true">Save</button>
    </div>
</template>

<script>
import cartComp from '@/components/cart-comp.vue';

    export default {
    components: { cartComp },
    data() {
        return {
            showModal: false,
        }
    },

    }
</script>

<style scoped>

</style>
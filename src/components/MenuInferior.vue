<script setup>
import { useScreen } from '@/composables/screen';
import CartPlus from 'vue-material-design-icons/CartPlus.vue';
import Account from 'vue-material-design-icons/Account.vue';
import Menu from 'vue-material-design-icons/Menu.vue';

const { isMobile } = useScreen();
</script>
<template>
 <div>
    <div v-if="isMobile" class="centerFoot">
        <Account />
        <CartPlus />
        <Menu />
    </div>
 </div>
</template>
<style scoped>
.centerFoot{
    display: flex;
    align-items: center;
    justify-content: center;
}
</style>
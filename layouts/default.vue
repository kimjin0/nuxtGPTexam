<template>
    <div>
        <span>
            <NuxtLink to="/">Home</NuxtLink>
        </span>
        <span class="marginleft">
            <NuxtLink to="counter">Counter <span>({{cart.length}})</span></NuxtLink>
        </span>
        <span class="marginleft">
            <NuxtLink to="profile">Profile</NuxtLink>
        </span>
    </div>
    <hr />
    <slot />
</template>
<style>
    .marginleft {
        margin-left: 10px;
    }
</style>
<script setup>
    const cart = useCart();
    console.log(cart.value.length);
</script>
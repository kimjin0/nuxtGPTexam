<template>
    <div>
        <span>
            <NuxtLink to="/">Home</NuxtLink>
        </span>
        <span class="marginleft">
            <NuxtLink to="counter">Counter</NuxtLink>
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
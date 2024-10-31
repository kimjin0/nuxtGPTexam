<template>
    <div>
        <span>
            <NuxtLink to="/">Home</NuxtLink>
        </span>
        <span class="endEle">
            <NuxtLink to="/counter">Counter</NuxtLink>
        </span>
    </div>
    <hr />
    <Counter />
</template>
<style>
    .endEle {
        margin-left: 10px;
    }
</style>
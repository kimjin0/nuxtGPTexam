<template>
    <main class="user-layout">
        <article class="sidebar" >
            <p class="box">Dashboard</p>
            <p class="box">Settings</p>
        </article>
        <section>
            <slot></slot>
        </section>
    </main>
</template>
<style>
.sidebar {
    display: flex;
    flex-direction: column;
}
.box {
    padding: 10px;
    margin: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
    width: 150px;
}
.user-layout {
    display: flex;
}
</style>
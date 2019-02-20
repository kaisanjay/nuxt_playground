<template>
    <div>
        <h1>products page</h1>

        <button @click="$router.push('/products/1')">product 1</button>
        <button @click="$router.push('/products/2')">product 2</button>

        <h2><strong>things on this page will be on every nested child pages. this is right next to 'product' folder </strong></h2>

        <nuxt-child />

        <h1>things after nuxt-child</h1>
    </div>
</template>

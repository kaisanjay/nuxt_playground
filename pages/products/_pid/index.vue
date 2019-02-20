<template>
    <div>
        <h1>
            <!-- if we have another dynamic route than _pid lets say we have _id then we will use $route.params.id -->

            <p style="color: red">nested route page Start</p>
            A single product id : {{ $route.params.pid }}
            <hr>

            <button @click="$router.push('/products')">Go back to products page</button>
            <p style="color: red">nested route page End</p>
        </h1>
    </div>
</template>

<script>
export default {
    validate(data) {
        console.log(data)
        return /^\d+$/.test(data.params.pid)
    }
}
</script>


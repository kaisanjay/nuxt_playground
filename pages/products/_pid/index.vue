<template>
    <div>
        <h1>
            <!-- if we have another dynamic route than _pid lets say we have _id then we will use $route.params.id -->
            A single product id : {{ $route.params.pid }}
        </h1>
    </div>
</template>

<script>
export default {
    validate(data) {
        console.log(data)
        return data.params.pid === '1'
    }
}
</script>


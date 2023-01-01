<template>
    <div class:="min-w-screen min-h-screen flex flex-row justify-center">
        <div class:="h-screen flex flex-col justify-center">
            <h1 class:="text-6xl font-bold">{{clock}}</h1>
        </div>
    </div>
</template>


<script lang="ts">
const clock = () => {
    const dt = new Date(); 
    return dt.toLocaleTimeString('en-US')
    setInterval(clock, 1000)
}
export default {
        name: 'index',
        data: []
}

console.log(clock)
</script>

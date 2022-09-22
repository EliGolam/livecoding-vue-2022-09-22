<template>
<div>
    <div 
        class="generic"
        :class="{ active: activeClass}" 
        @click="sayHi">I'm Generic
        <input v-model="text" class="inner" type="text" placeholder="I'm Inner within Generic" />
    
        <div class="box-1 inner">Box 1</div>
        <div class="box-2">Box 2</div>
    </div>
    <input v-model="text" class="inner" type="text" placeholder="I'm Inner Outside of Generic" />
    
    
</div>
</template>


<script>
export default {
    name: "FirstComponent",

    data() {
        return {
            activeClass: false,
        }
    },

    methods: {
        sayHi() {
            console.log("Hello!");
            this.activeClass = !this.activeClass;
        }
    }
} 
</script>

<style lang="scss" scoped>
$new-clr: aquamarine;
$another-clr: yellow;
$more-clr: lightblue;

@mixin ac-square {
    width: 100px;
    aspect-ratio: 1 / 1;
    margin: 1rem auto;
    border-radius: .7em;
}

@mixin circle {
    border-radius: 100vh;
}

.generic {
    background-color: $another-clr;

    .inner {
        background-color: $more-clr;
    }

    &.active {
        background-color: $new-clr;
    }
}

.inner {
    background-color: whitesmoke;
}

.box-1 {
    @include ac-square();
}

.box-2 {
    @include ac-square();
    @include circle();
    background-color: aquamarine;
}
</style>
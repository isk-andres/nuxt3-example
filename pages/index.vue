<template>
    <div>
        <h1 class="title"><span class="span-guapo"> Welcome</span>  to the home page <span>test</span></h1>
        <AppAlert>
            {{test2}}
            {{external}}
        </AppAlert>
        <button class="button is-primary" @click="external = 'yellow'"> CHANGE

        </button>
    </div>
</template>

<script setup lang="ts">
    import {ref} from 'vue';
    import {external} from '../test';
    const test2 = ref<string>('COMPONENT REF');
    const colorStyle  = ref<string>('blue');
</script>

<style lang="scss">
.title {
    .span-guapo {
        color: $vartest;
    }
    span {
        color: v-bind(colorStyle);
    }
}
</style>
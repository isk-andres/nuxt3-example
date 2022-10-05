<template>
    <div>
        <h1 class="title">Welcome to the ABOUT</h1>
        <AppAlert>
            {{external}}
        </AppAlert>
    </div>
</template>

<script setup lang="ts">
    import {external} from '../test';
</script>
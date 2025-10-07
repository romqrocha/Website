<script setup lang="ts">

interface Props {
    title: string
    postURL: string
    date: string
    tags: string[]
    subtitle: string
    thumbnailURL?: string
}

const props = defineProps<Props>()

</script>

<template>
    <div>
        <img src=""/>

        <a :href="props.postURL" :title="props.title">
            <h2 class="text-3xl font-bold underline">
                {{ props.title }}
            </h2>
        </a>
        

        <time datetime="">
            {{ props.date }}
        </time>

        <ul v-for="(tag, index) in props.tags" :key="index">
            <li>
                <span class="bg-green-100 animate-spin">
                    {{ tag }}
                </span>
            </li>
        </ul>

        <p>
            {{ props.subtitle }}
        </p>
    </div>
</template>

<style scoped>

</style>

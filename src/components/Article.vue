<template>
    <div class="article">
        <div class="pt-12 pl-12">
                <router-link 
                class="headline amber--text font-weight-black"
                :to="'/blog/' + slug">
                     {{ articleTitle }}
                </router-link>
            <p>
                {{ articleDate }} • ☕️ {{ articleTimeToRead }} min read
            </p>
            <p class="title font-weight-medium">
                {{ articleSubitle }}
            </p>
            <v-divider/>
        </div>
    </div>
</template>

<script>
export default {
    name:'Article',
    props:{
        slug:[String],
        articleTimeToRead:[Number],
        articleDate:[String],
        articleTitle:[String],
        articleSubitle:[String]

    }
}
</script>
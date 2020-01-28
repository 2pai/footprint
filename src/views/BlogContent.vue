<template>
    <div class="pt-12">
        <router-link to="/">⬅ Back</router-link>
        <v-rows
        no-gutters
        >
            <v-col
                md="7"
                offset-md="1"
            >
        <p class="display-1 font-weight-medium">
            Bagaimana cara berkontribusi ke ekosistem opensource
        </p>
            <VueShowdown
            :markdown="source"
            :options="{ emoji: true }"/>
      </v-col>
        </v-rows>

    </div>
</template>
<script>
import MarkdownFile from "!raw-loader!../../contents/markdown/kontribusi-opensource.md"

export default {
    name:'BlogContent',
    data:function(){
        return{
            source:MarkdownFile

        }
    }
    
}
</script>
<style>
img {
    width:100%;
    height:100%;
    display:block;

}
em {
  text-align: center;
}
</style>
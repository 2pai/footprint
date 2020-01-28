<template>
    <v-container class="pt-12">
              <v-row class="pb-8">
                <v-col cols="8">
                <blockquote class="blockquote headline pt-10">
                  Personal blog by Iqbal Syamil Ayasy<br>
                  Topic that i loved  
                  <kbd>#devops</kbd> <kbd>#cloudnative</kbd> <kbd>#opensource</kbd><br>
                  <p class="title font-weight-light"> All post blog made by pull request</p>
                </blockquote>
                </v-col>
                <v-col cols="4">
                  <v-avatar size="256">
                    <img src="https://user-images.githubusercontent.com/22183588/72966094-976a6880-3df0-11ea-9197-4c90bf7f6f1b.jpg"  alt="me">
                  </v-avatar>
                </v-col>
              </v-row>
          <v-divider light="true"/>
          <Article 
          v-for="content in this.listArticle"
            :key="content.id"
            :slug="content.id"
            :articleTimeToRead="content.time"
            :articleTitle="content.title"
            :articleDate="content.date"
            :articleSubitle="content.description"
          />
          </v-container>
</template>
<script>
import json from "../../contents/blog.json";
import Article from '../components/Article'
export default {
    name:'Blog',
    data:function(){
        return {
            articleTitle:"Hello world",
            articleSubitle:"Kenapa sih kita harus berkontribusi ke open source?",
            articleDate:"January 11, 2020",
            listArticle:json.contents
        }
    },
    components:{
        Article
    }
}
</script>
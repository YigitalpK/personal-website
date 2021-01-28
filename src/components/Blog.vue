<template>
<div class="blog">
    <div class = "posts" v-for="post in posts" :key="post.id">
        <div class = "post">
            <div class = "header"> <h2>{{ post.caption }}</h2> </div>
            <div class = "description"> {{post.description}} </div>
            <div class = "post-text"> {{post.postText}} </div>
            <div class = "post-date"> {{post.postDate}} </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
  name: 'Blog',
  data(){
      return {
         posts : [
          { 
              id : 1,
              caption : "How to do something with another thing?",
              postText: "There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable. If you are going to use a passage of Lorem Ipsum, you need to be sure there isn't anything embarrassing hidden in the middle of text. All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary, making this the first true generator on the Internet. It uses a dictionary of over 200 Latin words, combined with a handful of model sentence structures, to generate Lorem Ipsum which looks reasonable. The generated Lorem Ipsum is therefore always free from repetition, injected humour, or non-characteristic words etc.",
              description : "This is the best place to learn...",
              postDate : "11-03-2021",
          },
          {
              id : 2,
              caption : "Learning Vue.js With Berkay Kiran",
              postText: "There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable. If you are going to use a passage of Lorem Ipsum, you need to be sure there isn't anything embarrassing hidden in the middle of text. All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary, making this the first true generator on the Internet. It uses a dictionary of over 200 Latin words, combined with a handful of model sentence structures, to generate Lorem Ipsum which looks reasonable. The generated Lorem Ipsum is therefore always free from repetition, injected humour, or non-characteristic words etc.",
              description : "We are the best developers ever...",
              postDate : "test2",
          },
          {
              id : 3,
              caption : "I'm running out of ideas. Please gimme some.",
              postText : "There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable. If you are going to use a passage of Lorem Ipsum, you need to be sure there isn't anything embarrassing hidden in the middle of text. All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary, making this the first true generator on the Internet. It uses a dictionary of over 200 Latin words, combined with a handful of model sentence structures, to generate Lorem Ipsum which looks reasonable. The generated Lorem Ipsum is therefore always free from repetition, injected humour, or non-characteristic words etc.",
              description : "I'm not that creative :(",
              postDate : "test3",
          },
      ]
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.blog{
    max-width: 800px;   
    padding : center;
    margin-left: 700px;
    margin-right:auto;
}
.header{
    font-size : 25px;
}
.description{
    margin-top: -20px;
    margin-bottom: 15px;
    margin-left: 20px;
}
.post-text{
    font-style: italic;
}
.post-date{
    padding: auto;
    margin-top:10px;
    margin-left: 720px;
}

</style>

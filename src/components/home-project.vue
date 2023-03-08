<template lang="pug">
include ../assets/pugmix/mixin.pug

section.container
    +CreateH("projects",true)
    .project-list
        +CreatCard("../static/image/work1.jpg","HTML SCSS Python","Myproject","описание","Live <~>",true,"Cached >=")
        +CreatCard("../static/image/work1.jpg","HTML SCSS Python","Myproject","описание","Live <~>",false,"Cached >=")
        +CreatCard("../static/image/work1.jpg","HTML SCSS Python React Express Discord.js Flas Node.js Flask","Myproject","описание","Live <~>",false,"Cached >=")
</template>


<script>

export default{
    name:"home-project"
}

</script>
<style scoped lang="scss">
.project-list{
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
  
    padding-bottom: 50px;
}
</style>
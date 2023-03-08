<template lang="pug">
header.header.container 
    nav.header__navigator 
        ul.header__list
            li.header__item 
                span { 
                span.header__name Vladislav
                span :
                span.header__nik Xarn0 
                span }
               
            li.header__item
                router-link(:to="{name:'home'}").
                    home
            li.header__item
                router-link(:to="{name:'works'}").
                    works   
                
            li.header__item
                router-link(:to="{name:'about'}").
                        about-me
               
            li.header__item
                router-link(:to="{name:'contact'}").
                        contacts
                
            li.header__item
                select.header__select
                    option(value="ru") ru 
                    option(value="en") en



</template>

<script>
export default {
    name: "my-header"
}
</script>

<style lang="scss" >
@import "@/assets/scss/style";

li.header__item+li.header__item {
    &::before {
        content: "#";
        font-weight: 400px;
        color: $color-header-link-icon;
    }
}

li.header__item:last-child {
    
    &::before {
        content: '' !important;
        
    }
}
</style>
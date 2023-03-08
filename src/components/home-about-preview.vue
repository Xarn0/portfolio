<template lang="pug">
include ../assets/pugmix/mixin.pug
section.homeAbouPreview.container
    .homeAbouPreview__container
        .homeAbouPreview__header
            +CreateH("about-me")
        .homeAbouPreview__content.homeAbouPreview__content-list
            .homeAbouPreview__text
                h3 Hello, i’m Xarn0 !
                p.
                   I’m a self-taught front-end developer based in Kyiv, Ukraine. I can develop responsive websites from scratch and raise them into modern user-friendly web experiences.
                p.
                    Transforming my creativity and knowledge into a websites has been my passion for over a year. I have been helping various clients to establish their presence online. I always strive to learn about the newest technologies and frameworks. 
            .homeAbouPreview__img
                img(src="../static/image/homeaboutpreview.png", alt="4", srcset="")   

</template>
<style scoped lang="scss">
.homeAbouPreview{
    padding-bottom: 20px;
    &__content{
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
      
    }
    &__text{
        width: 500px;
        text-align: left; 
        display: flex;
        flex-direction: column;
        justify-content: center;
        >h3{
            margin-bottom: 30px;
        }
        >p{
            margin-bottom: 23px;
        }
    }
    &__img{
       width: 300px;
       margin-top: -80px;
       position: relative;
       &::before{
        content: "";
        width: 70px;
        height: 70px;
        top: 20px;
        left: -10px;
        background: url(../static/image/homeaboutafter.png);
        background-size: cover;
        position: absolute;
       }
       &::after{
        content: "";
        
        width: 76px;
        height: 40px;
        top: 50%;
        right: 0;
        background: url(../static/image/homeaboutafter.png);
        background-size: cover;
        position: absolute;
       }
       
        img{
            width:100%;
            object-fit: cover;
            display: block;
            
            
           
        }
      
    } 
}


</style>
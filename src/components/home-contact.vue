<template lang="pug">
include ../assets/pugmix/mixin.pug
section.homeContacts.container
    .homeContacts__container
        .homeContacts__header 
            +CreateH("contacts")
        .homeContacts__content.public_margin
            .homeContacts__text. 
                I’m interested in freelance opportunities. However, if you have other request or question, don’t hesitate to contact me
            .homeContacts__contacts
                .homeContacts__ItemContact
                    contacts
</template>

<script>

import contacts from "@/components/home-mini-components/contact-react.vue"

export default{
    components:{
        contacts
    }


}

</script>




<style lang="scss" scoped>
.homeContacts{
    margin-top: 20px;
    &__content{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    &__text{
        width: 505px;
        text-align: left;
        font-weight: 500;
    }
}



</style>
<template>
    <div class="HeaderContent">
        <div class="header_content_inner">
            <HeaderContentInnerItem v-for="(data,i) in header_content_inner_config" :key="i" :data="data"/>
        </div>
        <div class="header_content_user">
            <p>Armen <br> Hakobyan</p>
             <q-avatar>
                <img src="https://cdn.quasar.dev/img/avatar.png">
            </q-avatar>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .HeaderContent{
        display: flex;
        padding: 10px;
    }
    .header_content_inner{
        display: grid;
        grid-template-columns: auto auto auto;
        grid-gap: 20px;
    }
    .header_content_user{
        display: flex;
        align-items: center;
    }
    .header_content_user p{
        margin: 0 20px;
        font-weight: bold;
        text-align: center;
    }
    .header_content_user .q-avatar{
        width: 70px;
        height: 70px;
    }
</style> 


<script>
import HeaderContentInnerItem from "./HeaderContentInnerItem"
// const header_content_inner_config = [
//     {
//         id: 1,
//         name: "Total activations", 
//         quantity: 56,
//         buttonText : "Get activations"
//     },
//     {
//         id: 2,
//         name: " Total earings", 
//         quantity: 100,
//         buttonText : "Witdraw found"
//     },
// ]

export default {
    name: "HeaderContent",
     data() {
        return {
            header_content_inner_config: [
                {
                    name: "Total activations", 
                    quantity: 56,
                    buttonText : "Get activations"
                },
                {
                    name: "Total earings", 
                    quantity: 100,
                    buttonText : "Witdraw found"
                },
            ]
        };
    },
    components: {HeaderContentInnerItem}
}
</script>

<template>
    <Layout>
        <template #header>
            <Header></Header>
        </template>
        <template #resume>
            <Resume
                :label = "'Ahorro total'"
                :total-amount="100000"
                :amount="amount"
            
            ></Resume>
        </template>
        <template #movements>
            <Movementes></Movementes>
        </template>
    </Layout>    
</template>
<script>
import Layout from "./Layout.vue";
import Header from "./Header.vue";
import Resume from "./Resume/Index.vue";
import Movements from "./Movements.vue";
export default{
    components:{
        Layout,
        Header,
        Resume,
        Movements
    },
    data(){
       return{
        amount: null,
       }
    },
}
</script>
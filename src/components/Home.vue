<template>
   <v-container fluid>
       <div class="pills">
           <Pill v-for="word in groupedWords" :key="word.name"
                :name="word.name" :amount="word.amount" />
       </div>
   </v-container>
</template>

<script>
import Pill from "./Pill";

export default {
    components: {Pill},
    data: function(){
        return {
            groupedWords:[
                {name: "you", amount: 900},
                {name: "he", amount: 853},
                {name: "i", amount: 1234}
            ]
        }
    }

}
</script>

<style>

</style>
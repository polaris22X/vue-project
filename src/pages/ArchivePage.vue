<template>
    <card-list :archives="archives" />
</template>

<script>
import CardList from '../components/CardList.vue'
export default {
    name: 'ArchivePage',
    components:{
        CardList
    },
    data(){
        return{
            archives:[
                {
                    date: "25-05-2020",
                    time: "17:00",
                    tasks: [
                        { id: 1, title: "ITEM : A", status: "done" },
                        { id: 2, title: "ITEM : B", status: "done" },
                    ]
                },
                {
                    date: "26-05-2020",
                    time: "17:00",
                    tasks: [
                        { id: 1, title: "ITEM : C", status: "done" },
                        { id: 2, title: "ITEM : D", status: "done" },
                    ]
                }
            ]
        }
    }
}
</script>
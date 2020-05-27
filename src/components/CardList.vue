<template>
    <div class="container">
        <div class="card" v-for="archive in archives" :key="archive.id">
            <h3>{{ archive.date }} : {{ archive.time }}</h3>
            <ul v-for="task in archive.tasks" :key="task.id">
                <li>{{ task.id }} - {{ task.title }}</li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardList',
    props: ['archives']
}
</script>

<style scoped>
h3{
    border-bottom: 2.5px solid pink;
    padding-bottom: 8px;
    color: whitesmoke;
}
.card{
    padding: 8px 0;
    background-color: black;
    width: 50%;
    height: auto;
    border-radius: 20px;
    border: 2.5px solid pink;
    margin: 8px auto;
    color: whitesmoke
}
li{
    list-style: none;
}
</style>
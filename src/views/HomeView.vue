<template>
  <div class="home">
      <div v-if="tasks.length">
            <div v-for="task in tasks" :key="task.id">
                  <!-- <p>{{task.title}}</p> -->
                  <SingleTask :task="task"/>
            </div>
      </div>
  </div>
</template>

<script>
// @ is an alias to /src
import SingleTask from '../components/SingleTask.vue'
export default {
  name: 'HomeView',
  components: {
      SingleTask
  },
  data(){
    return{
        tasks:[]
    }
  },
  mounted(){
      fetch('http://localhost:3000/tasks').then(res=>res.json()).then(data=>this.tasks=data).catch(err=>console.log(err.message));
  }
}
</script>

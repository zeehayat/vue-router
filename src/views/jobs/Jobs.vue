<template>
<h1>Jobs</h1>
<div v-for="job in jobs" class='jobs'>
<router-link :to="{name: 'JobDetails',params:{id:job.id}}">
<h2>{{job.title}}</h2>
</router-link>
</div>
</template>

<script>
export default {
  name:'Jobs',
  data(){
    return {
      jobs:[
        {title: 'Ninja UI Designer', id:1,description:'Lori'},
        {title: 'Ninja Web Developer', id:2,description:'Ipsum'},
        {title: 'Ninja Web Designer', id:3,description:'Dora'},
      ]
    }
  }
}
</script>
<style>
.jobs h2{
  background-color:#f4f4f4;
  padding:20px;
  margin: 10px auto;
  border-radius:5px;
  color:#4444;
  max-width:600px;
}
.jobs h2:hover {
background:#dddd
}
.jobs a {
  text-decoration:none;
}
</style>
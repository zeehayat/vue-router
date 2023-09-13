<template>
<h1>Jobs</h1>
<div v-for="job in jobs">
<h2>{{job.title}}</h2>
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
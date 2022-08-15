<script >
import axios  from 'axios';
export default{
  data(){
    return {
      URL:"https://jsonplaceholder.typicode.com/todos",
      datas:[]
    }
  },
  methods:{
    onGetData(){
      axios.get(this.URL).then((res)=>{
        this.datas = res.data
        console.log(this.datas);
      })

    }
  },
  mounted(){
    this.onGetData()
  }

}
</script>

<template>
<div class="card-group">
  <div class="card" v-for="value in datas" :key="value">
    <div>{{value.title}}</div>
    <div>{{value.completed}}</div>
  </div>
</div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
.card-group{
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
.card{
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
  margin: 20px;
  padding: 5px;
  border-radius: 5px;
  border-left: solid purple;
  width: 25%;
}
</style>

<template>
  <div class="hello">

    <ul>
      <li v-for="item in items" :key="item.name">
        {{ item.name }} - {{ item.age }}
      </li>
    </ul>

    <ul>
      <li v-for="(val, key, index) in person" :key="index">
           {{ index }} - {{ key }} - {{ val }}
      </li>
    </ul>

  </div>
</template>

<script>

export default {
  name: 'HelloWorld',
  data() {
    return {     
      msg : '반갑습니다.',
      author : '밥 아저씨',
      age : 30,
      article : '<strong>hello world!!</strong>',
      info : {
                job : 'developer',
                marry : 'not marry'
             },
      seen : false,
      isActive : true,
      url : 'http://google.com',
      items : [
        {name: 'red', age:15},
        {name: 'blue', age:25},
        {name: 'green', age: 20},
        {name: 'yello', age: 10}
      ],

      person : {
        name : 'bob',
        age : 25,
        location : 'seoul'
      }

    }
  }

  // props: {
  //   msg: String
  // }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

</style>

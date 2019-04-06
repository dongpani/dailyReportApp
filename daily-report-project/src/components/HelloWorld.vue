<template>
  <div class="hello">

    <ol>
      <li> <button @click="updateScore(1)">클릭하세요</button> </li>
      <li> <button @click.once="updateScore(1)">클릭하세요(once)</button> </li>
    </ol>

    <input type="text" @keyup.enter="keyup">

  </div>
</template>

<script>

export default {
  name: 'HelloWorld',

  // 이벤트
  methods: {
    updateScore(score) {
      console.log('update', score);
    },
    keyup() {
      console.log('key');
    }
  },

  // 데이터
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

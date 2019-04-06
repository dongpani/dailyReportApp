<template>
  <div class="hello">
    <h1>메세지 : {{ msg }}</h1>
    <h2>이름 : {{ author }}</h2>

    <p :class="{active : isActive}"> active </p>
    <p :style="{color:'red'}">스타일 바인드</p>

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
      url : 'http://google.com'
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

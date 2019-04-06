<template>
  <div class="hello">
    <h1>메세지 : {{ msg }}</h1>
    <h2>이름 : {{ author }}</h2>
    <p> 나이 : {{ age }}</p>
    <p v-html="article"></p>
    <p>간략 소개 : {{ info.job }}, 결혼 : {{ info.marry }} </p>
    <p v-if="seen">보인다</p>
    <p v-else>보이지 않음</p>
    <p v-show="seen">show</p>
    <p v-show="!seen">not show</p>
    <p><a v-bind:href="url" target="_brank">구글 페이지</a></p>
    <p><a :href="url" target="_brank">구글 페이지</a></p>
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

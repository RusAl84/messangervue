<template>
  <v-container>

    <div id="example-1">
      <button v-on:click="counter += 1">+1</button>
      <p>Кнопка выше была нажата {{ counter }} раз</p>
    </div>

    <v-btn
        class="mx-2"
        fab
        dark
        small
        color="pink"
    >
      <v-icon dark>
        mdi-heart
      </v-icon>
    </v-btn>
    </v-container>
</template>

<script>
export default {
  // Модель данных страницы
  data: () => {
    return {
      counter: 0,
      username: '',
      message: '',
      // messages: [
      //   {"username": "fddffdfdfd", "text": "texttexttexttexttexttext1", "timestamp": "2020-10-15T17:05:12.417897Z"},
      //   { "UserName":"RusAl","MessageText":"Privet na sto let!!!","TimeStamp":"2021-03-05T18:23:10.932973Z"},
      messages: [],
      intervalCtx: null,
      lastMsgID: 0,
    }
  },
}

</script>

<style scoped>

</style>
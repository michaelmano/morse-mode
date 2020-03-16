<template>
  <section class="p-4">
      <input type="text" v-model="text" class="w-full p-2 border shadow"/>
      <div v-for="(value, key) in keys" :key="`key-${value}`">
          <span v-html="key"/> : <span v-html="value"/>
      </div>
  </section>
</template>
<script>
export default {
  name: 'Keyboard',
  data() {
    return {
      text: '',
      keys: {
        A: '.-',
        B: '-...',
        C: '-.-.',
        D: '-..',
        E: '.',
        F: '..-.',
        G: '--.',
        H: '....',
        I: '..',
        J: '.---',
        K: '-.-',
        L: '.-..',
        M: '--',
        N: '-.',
        O: '---',
        P: '.--.',
        Q: '--.-',
        R: '.-.',
        S: '...',
        T: '-',
        U: '..-',
        V: '...-',
        W: '.--',
        X: '-..-',
        Y: '-.--',
        Z: '--..',
        '0': '-----',
        '1': '.----',
        '2': '..---',
        '3': '...--',
        '4': '....-',
        '5': '.....',
        '6': '-....',
        '7': '--...',
        '8': '---..',
        '9': '----.',
        '.': '.-.-.-',
        ',': '--..--',
        '?': '..--..',
        '=': '-...-',
      },
    };
  },
  watch: {
      text(val) {
          console.log(val);
      },
  },
};
</script>

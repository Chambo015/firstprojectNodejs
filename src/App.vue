<template>
  <div id="app">
    <div class="mb-1 flex justify-center">
      <p  class=" text-red-700" v-if="counter < 0" >
        {{ counter }}
      </p>
      <p v-else >
        {{ counter }}
      </p>
    </div>
    <div class="flex justify-center items-center min-h-full font-mukta">
      <button @click="counter--">
        <span
          class="text-white bg-black rounded-full h-9 w-9 inline-block mr-1"
        >
          <i class="fa-solid fa-minus leading-9"></i>
        </span>
      </button>
      <button @click="counter++">
        <span
          class="text-white bg-black rounded-full h-9 w-9 inline-block mr-1"
        >
         <i class="fa-solid fa-plus leading-9"></i>
        </span>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
  data() {
    return {
      counter: 0,
    };
  },
};
</script>



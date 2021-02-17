<template>
    <nav class="-mt-16 py-5 bg-white flex">
        <div class="flex w-1/2">
            <img class="h-16 -mt-3 -mb-3 ml-3" src="../assets/logo-vuejs-min.png" />
        </div>
        <div class="flex w-1/2 justify-end">
            <button class="bg-green text-white border-2 border-solid border-green focus:outline-none hover:bg-white hover:text-green hover:border-green rounded-full pl-5 pr-5 mr-3" @click="aboutMore">About More</button>
        </div>
    </nav>
</template>

<script>
export default {
  name: "PxHeader",

  methods: {
      aboutMore () {
          window.location.href = "https://vuejs.org/";
      }
  }
};
</script>

<script setup>
import Test from './components/test.vue';
import { test } from './store';
import MessageBox from './components/MessageBox.vue';
import { icons } from './icons';
import Icon from './components/Icon.vue';
function add() {
  test.value += 1
}

</script>

<template>
  <div class="h-screen w-screen bg-slate-900 grid grid-rows-12">
    <div class="msgsbox w-screen p-4 row-span-10">
      <MessageBox name="Vampire.js" time="12:00 AM" msg="lorem ipsum dor amet miti lmao ded no lmao lmao lelellellel" />

    </div>
    <div class="textbox bg-slate-900 border-t-2 border-t-slate-800 p-8 row-span-2 flex">
      <div class="flex justify-between items-center w-full">
        <div class="flex items-center">
          <div class="btn p-2 rounded-full  text-white hover:bg-slate-800 transition-all ">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
              stroke="currentColor" class="size-6">
              <path stroke-linecap="round" stroke-linejoin="round"
                d="m11.25 11.25.041-.02a.75.75 0 0 1 1.063.852l-.708 2.836a.75.75 0 0 0 1.063.853l.041-.021M21 12a9 9 0 1 1-18 0 9 9 0 0 1 18 0Zm-9-3.75h.008v.008H12V8.25Z" />
            </svg>

          </div>
          <div class="btn ml-3 p-2 rounded-full  text-white hover:bg-slate-800 transition-all ">
            <Icon icon="info" />
          </div>
        </div>
        <input type="text" placeholder="Type here ..." class="p-4 w-full mx-5 text-slate-100 rounded-xl bg-slate-800 text-xl">
        <div class="btn p-2 rounded-full  text-white hover:bg-slate-800 transition-all ">
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
            stroke="currentColor" class="size-6">
            <path stroke-linecap="round" stroke-linejoin="round"
              d="M6 12 3.269 3.125A59.769 59.769 0 0 1 21.485 12 59.768 59.768 0 0 1 3.27 20.875L5.999 12Zm0 0h7.5" />
          </svg>

        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>

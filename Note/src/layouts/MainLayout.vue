<style>
.cls-1 {
  fill: #41416e;
}

.bg-whitesmoke {
  background-color: #FFFFFF;
}
</style>
<template>
  <q-layout view="lHr lpR lfr">
    <q-header flat class="border border-grey bg-whitesmoke  text-black">
      <q-toolbar class="">
        <q-toolbar-title @click="toggleLeftDrawer" class="text-3xl text-black font-bold">
          Software as a Service
        </q-toolbar-title>
        <div class="flex-row inline-flex">
          <svg viewBox="0 0 24 24" class="h-6" id="magicoon-Regular" xmlns="http://www.w3.org/2000/svg" fill="#000000">
            <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
            <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
            <g id="SVGRepo_iconCarrier">
              <defs>

              </defs>
              <title>comments</title>
              <g id="comments-Regular">
                <path id="comments-Regular-2" data-name="comments-Regular" class="cls-1"
                  d="M18,7.25h-.25V6A3.754,3.754,0,0,0,14,2.25H6A3.754,3.754,0,0,0,2.25,6V16a.75.75,0,0,0,.466.694A.741.741,0,0,0,3,16.75a.749.749,0,0,0,.536-.225L5.275,14.75H6.25V16A3.754,3.754,0,0,0,10,19.75h8.725l1.739,1.775A.749.749,0,0,0,21,21.75a.741.741,0,0,0,.284-.056A.75.75,0,0,0,21.75,21V11A3.754,3.754,0,0,0,18,7.25Zm-13.04,6a.75.75,0,0,0-.536.225l-.674.688V6A2.252,2.252,0,0,1,6,3.75h8A2.252,2.252,0,0,1,16.25,6v5A2.252,2.252,0,0,1,14,13.25Zm15.29,5.913-.674-.688a.75.75,0,0,0-.536-.225H10A2.252,2.252,0,0,1,7.75,16V14.75H14A3.754,3.754,0,0,0,17.75,11V8.75H18A2.252,2.252,0,0,1,20.25,11Z">
                </path>
              </g>
            </g>
          </svg>
          <svg viewBox="0 0 16 16" xmlns="http://www.w3.org/2000/svg" fill="#000000"
            class="h-6 bi bi-three-dots-vertical">
            <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
            <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
            <g id="SVGRepo_iconCarrier">
              <path
                d="M9.5 13a1.5 1.5 0 1 1-3 0 1.5 1.5 0 0 1 3 0zm0-5a1.5 1.5 0 1 1-3 0 1.5 1.5 0 0 1 3 0zm0-5a1.5 1.5 0 1 1-3 0 1.5 1.5 0 0 1 3 0z">
              </path>
            </g>
          </svg>
          <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="h-6">
            <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
            <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
            <g id="SVGRepo_iconCarrier">
              <path d="M19.8978 16H7.89778C6.96781 16 6.50282 16 6.12132 16.1022C5.08604 16.3796 4.2774 17.1883 4 18.2235"
                stroke="#1C274D" stroke-width="1.5"></path>
              <path d="M8 7H16" stroke="#1C274D" stroke-width="1.5" stroke-linecap="round"></path>
              <path d="M8 10.5H13" stroke="#1C274D" stroke-width="1.5" stroke-linecap="round"></path>
              <path
                d="M13 16V19.5309C13 19.8065 13 19.9443 12.9051 20C12.8103 20.0557 12.6806 19.9941 12.4211 19.8708L11.1789 19.2808C11.0911 19.2391 11.0472 19.2182 11 19.2182C10.9528 19.2182 10.9089 19.2391 10.8211 19.2808L9.57889 19.8708C9.31943 19.9941 9.18971 20.0557 9.09485 20C9 19.9443 9 19.8065 9 19.5309V16.45"
                stroke="#1C274D" stroke-width="1.5" stroke-linecap="round"></path>
              <path
                d="M10 22C7.17157 22 5.75736 22 4.87868 21.1213C4 20.2426 4 18.8284 4 16V8C4 5.17157 4 3.75736 4.87868 2.87868C5.75736 2 7.17157 2 10 2H14C16.8284 2 18.2426 2 19.1213 2.87868C20 3.75736 20 5.17157 20 8M14 22C16.8284 22 18.2426 22 19.1213 21.1213C20 20.2426 20 18.8284 20 16V12"
                stroke="#1C274D" stroke-width="1.5" stroke-linecap="round"></path>
            </g>
          </svg>
        </div>
      </q-toolbar>
      <span class="text-grey-5 mx-3">
        How to build a Saas application in 8 steps
      </span>
    </q-header>
    <q-drawer v-model="leftDrawerOpen" side="left" show-if-above bordered :height="350">
      <q-scroll-area class="fit" >

        <q-list>
          <q-item-label header>
            Username
          </q-item-label>


          <q-input ronnded dense outlined v-model="text" class="px-2 rounded-3xl">
            <template v-slot:append>
              <q-avatar>
                <img
                  src="https://plus.unsplash.com/premium_photo-1692468867066-d440f327ed36?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHwyN3x8fGVufDB8fHx8fA%3D%3D">
              </q-avatar>
            </template>
          </q-input>
          <div class="flex items-center justify-center">
            <q-btn-dropdown class="my-2 bg-blue text-white  text-start px-12" label="New Note" icon="note_alt">
              <q-list>
                <q-item clickable v-close-popup @click="onItemClick">
                  <q-item-section>
                    <q-item-label>Photos</q-item-label>
                  </q-item-section>
                </q-item>

                <q-item clickable v-close-popup @click="onItemClick">
                  <q-item-section>
                    <q-item-label>Videos</q-item-label>
                  </q-item-section>
                </q-item>

                <q-item clickable v-close-popup @click="onItemClick">
                  <q-item-section>
                    <q-item-label>Articles</q-item-label>
                  </q-item-section>
                </q-item>
              </q-list>
            </q-btn-dropdown>

          </div>

          <div class="w-full flex justify-between mt-3 px-3">
            <strong>
              4 notes
            </strong>
            <q-icon name="filter" />
          </div>

          <div class=" p-4 max-w-sm mx-auto rounded">
            <ul class="space-y-2">
              <li class="bg-white p-4 rounded-xl shadow" v-for="i in 35" :key="i">
                <h3 class="font-semibold">No-code development...</h3>
                <p class="text-xs text-gray-500">Mar 05, 2022, 3:06 AM</p>
              </li>

            </ul>
          </div>

          <q-separator />
        </q-list>
      </q-scroll-area>

    </q-drawer>
    <!-- <q-drawer v-model="rightDrawerOpen" side="right" show-if-above bordered>
      <q-scroll-area class="fit">


        <rightdrawer />
      </q-scroll-area>
    </q-drawer> -->

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';
import Rightdrawer from 'src/components/RightDrawer.vue';
export default defineComponent({
  // components: {
  //   Rightdrawer,
  // },
  setup() {
    const leftDrawerOpen = ref(false);
    const rightDrawerOpen = ref(false)

    return {
      simple: [
        {
          label: 'Satisfied customers (with avatar)',
          avatar: 'https://cdn.quasar.dev/img/boy-avatar.png',
          children: [
            {
              label: 'Good food (with icon)',
              icon: 'restaurant_menu',
              children: [
                { label: 'Quality ingredients' },
                { label: 'Good recipe' }
              ]
            },
            {
              label: 'Good service (disabled node with icon)',
              icon: 'room_service',
              disabled: true,
              children: [
                { label: 'Prompt attention' },
                { label: 'Professional waiter' }
              ]
            },
            {
              label: 'Pleasant surroundings (with icon)',
              icon: 'photo',
              children: [
                {
                  label: 'Happy atmosphere (with image)',
                  img: 'https://cdn.quasar.dev/img/logo_calendar_128px.png'
                },
                { label: 'Good table presentation' },
                { label: 'Pleasing decor' }
              ]
            }
          ]
        }
      ],
      text: ref('chijoke'),
      rightDrawerOpen,
      leftDrawerOpen,
      toggleRightDrawer() {
        rightDrawerOpen.value = !rightDrawerOpen.value
      },
      toggleLeftDrawer() {
        leftDrawerOpen.value = !leftDrawerOpen.value
      }
    }
  }
});
</script>

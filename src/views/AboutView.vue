<template>
  <main>
    <div class="xsm:my-16 xsm:w-screen antialiased max-h-max w-3/5">
      <h1
        class="xsm:w-full xsm:text-center xsm:m-0 xsm:text-2xl uppercase font-sans antialiased font-semibold xl:text-3xl"
        >About the creator</h1
      >
      <div class="xsm:mx-5 lg:mx-20 xl:mx-48 my-5 xsm:text-lg lg:text-xl">
        <p>
          {{ about.descr }}
          <a
            class="text-teal-700 hover:text-white hover:bg-teal-700 duration-300"
            :href="about.apiLink"
            >{{ about.apiLinkDesc }}</a
          >.
        </p>
      </div>
      <div class="xsm:mx-5 lg:mx-20 xl:mx-48 y-5 xsm:text-lg lg:text-xl">
        <p>
          {{ about.repoDescr }}
          <a
            class="text-teal-700 hover:text-white hover:bg-teal-700 duration-300"
            :href="about.githubProjectLink"
          >
            {{ about.githubProjectDesc }}
          </a>
          {{ about.contactDesc }}
        </p></div
      >
      <div class="xsm:mx-5 lg:mx-20 xl:mx-48 my-5 xsm:text-lg lg:text-xl">
        <p>
          <a
            class="text-teal-700 hover:text-white hover:bg-teal-700 duration-300"
            :href="about.portfolioLink"
          >
            {{ about.portfolioDesc }}
          </a>
          /
          <a
            class="text-teal-700 hover:text-white hover:bg-teal-700 duration-300"
            :href="about.linkedInLink"
          >
            {{ about.linkedInDesc }}
          </a>
          /
          <a
            class="text-teal-700 hover:text-white hover:bg-teal-700 duration-300"
            :href="about.githubLink"
          >{{ about.githubDescr }} </a
          >
        </p>
        <p>
          Email:
          <a
            class="text-teal-700 hover:text-white hover:bg-teal-700 duration-300"
            :href="about.emailLink"
          >{{ about.emailDescr }}</a
          >
        </p></div
      >
    </div>
  </main>
</template>

<script lang="ts">
import { about } from '../data/about';

export default {
  data() {
    return {
      about: about,
    };
  },
};
</script>

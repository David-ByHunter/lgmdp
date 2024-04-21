<script setup lang="ts">
import { name, description } from '@/components/data/info'
import { donate } from '@/components/data/links'
import DescriptionMDP from '@/components/DescriptionMDP.vue'
import ProfilePicture from '@/components/ProfilePicture.vue'
import LinkBtn from '@/components/LinkBtn.vue'
import Separator from '@/components/SeparatorLine.vue'
import FooterIcons from '@/components/FooterIcons.vue'
</script>

<template>
  <div class="flex flex-col items-center gap-y-6">
    <ProfilePicture class="mt-8" />
    <h1 class="font-black text-xl text-center uppercase">{{name}}</h1>
    <FooterIcons />
    <Separator />
    <DescriptionMDP :text="description" />
    <Separator />
    <LinkBtn
      :title="donate.title"
      :link="donate.link"
      :alt="donate.alt"
    ></LinkBtn>
  </div>
</template>

<template>
  <div>
    <div class="border">
      <!--? child componente prop göndermek -->
      <Title title="Interview Preparation prop 1" />
      <Title :title="title2" />
      <!--? child componente prop göndermek -->
      <!--? slot mantığı -->
      <Title>
        <h1>Interview Preparation slot mantığı</h1>
      </Title>
      <Title>
        <h1 slot="title">Interview Preparation named slot mantığı</h1>
      </Title>
    </div>
    <!--? slot mantığı -->
    <Counter />
    <Product />
    <User />
    <Test />
    <PiniaExample />
    <div class="border">
      <h1>v-if & v-show farkı</h1>
      <TeleportExample />
      <TeleportExample2 />
    </div>
    <Binding />
    <EmitParent />
    <ProvideInjectParent />
    <Directive />
  </div>
</template>

<script setup>
import { ref } from "vue";
import Title from "../components/Title.vue";
import Counter from "../components/Counter.vue";
import User from "../components/User.vue";
import Product from "../components/Product.vue";
import Test from "../components/Test.vue";
import PiniaExample from "../components/PiniaExample.vue";
import TeleportExample from "../components/TeleportExample.vue";
import TeleportExample2 from "../components/TeleportExample2.vue";
import Binding from "../components/Binding.vue";
import EmitParent from "../components/EmitParent.vue";
import ProvideInjectParent from "../components/ProvideInjectParent.vue";
import Directive from "../components/Directive.vue";

const title2 = ref("Interview Preparation prop 2");
</script>

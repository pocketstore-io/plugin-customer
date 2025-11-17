<template>
  <div />
</template>

<script lang="ts" setup>
import { onMounted } from "vue";
import { useRouter } from "vue-router";
import { usePocketBase } from "~/utils/pocketbase";

const router = useRouter();
const pb = usePocketBase();

onMounted(() => {
    pb.authStore.clear();
    router.push("/");
});
</script>

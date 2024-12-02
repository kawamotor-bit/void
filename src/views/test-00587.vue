<script setup>
import { useLockScreen } from 'viy-ui';
import { useI18n } from 'vue-i18n';

const { t } = useI18n();
const { lockScreen } = useLockScreen();

defineOptions({
  name: 'test-00587',
});

const form = ref();

const formData = reactive({
});
</script>

<template>
  <VueForm ref="form" v-loading="lockScreen" :model="formData">
    <VueText id="viy2Text_7Nb4G" ref="viy2Text_7Nb4G" :style="{ width: '100%', display: 'inline-block' }">
      Hello World!
    </VueText>
  </VueForm>
</template>

<template>
  <section class="home-view">
    <h1>This is an home page</h1>


    <section>
      <RunaiRadio> default</RunaiRadio>
      <RunaiRadio color="positive"> positive</RunaiRadio>
      <RunaiRadio color="success"> success</RunaiRadio>
      <RunaiRadio color="negative"> negative</RunaiRadio>
      <RunaiRadio color="warning"> warning</RunaiRadio>
      <RunaiRadio color="info"> info</RunaiRadio>
    </section>


    <br />
    <hr />
    <br />

    <section>
      <RuaniChip> default</RuaniChip>
      <RuaniChip color="positive"> positive</RuaniChip>
      <RuaniChip color="success"> success</RuaniChip>
      <RuaniChip color="negative"> negative</RuaniChip>
      <RuaniChip color="warning"> warning</RuaniChip>
      <RuaniChip color="info"> info</RuaniChip>
    </section>

    <br />
    <hr />
    <br />

    <section>
      <RuaniBtn> default </RuaniBtn>
      <RuaniBtn color="positive"> positive</RuaniBtn>
      <RuaniBtn color="success"> success</RuaniBtn>
      <RuaniBtn color="negative"> negative</RuaniBtn>
      <RuaniBtn color="warning"> warning</RuaniBtn>
      <RuaniBtn color="info"> info</RuaniBtn>
    </section>
  </section>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import RuaniChip from 'runpi-core/src/components/runai-chip/runai-chip.vue';
import RuaniBtn from 'runpi-core/src/components/runai-btn/runai-btn.vue';
import RunaiRadio from 'runpi-core/src/components/runai-radio/runai-radio.vue';

export default defineComponent({
  components: {
    RuaniChip,
    RuaniBtn,
    RunaiRadio,
  }
})
</script>
<style lang="scss" scoped>
.home-view {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}
</style>

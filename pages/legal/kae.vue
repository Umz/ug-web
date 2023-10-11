<template>

  <LegalContent
    :game-name="game"
    :game-terms="terms"
    :game-privacy="privacy"
  />
  
</template>

<style lang="css">
  @import url('~/assets/css/legal.css');
</style>

<script>
import { LegalContent } from "#components";

export default {
  data() {
    return {
      game: 'Killer Ant Empire',
      terms: "Loading terms..",
      privacy: "Loading privacy.."
    }
  },
  setup() {
    const { data, error } = useFetch(
      "/json/kae-legal.json"
    );
    return { data, error };
  },
}
</script>
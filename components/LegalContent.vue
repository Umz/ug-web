<template>

    <div class="contained-content">

        <div id="legal-heading">
            <h1>{{ gameName }}</h1>
        </div>

        <section id="terms-of-use">
            <h2>Terms of Use</h2>
            <div class="legal-content">
                {{ gameTerms }}
            </div>
        </section>

        <div class="divider"></div>

        <section id="privacy">
            <h2>Privacy Policy</h2>
            <div class="legal-content">
                {{ gamePrivacy }}
            </div>
        </section>

    </div>

</template>

<style lang="css">
  @import url('~/assets/css/legal.css');
</style>

<script>
export default {
    name: 'LegalContent',
    props: [
        'gameName',
        'gameTerms',
        'gamePrivacy'
    ]
}
</script>

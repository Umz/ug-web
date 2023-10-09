<template>
    <div>
        <Header />
        <slot />
        <Footer />
    </div>
</template>

<script>
import { Header, Footer } from '#components';
</script>
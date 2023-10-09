<template>
    <div>
        <Header />
        <div id="page-content">
            <slot />
        </div>
        <Footer />
    </div>
</template>

<script>
import { Header, Footer } from '#components';
</script>
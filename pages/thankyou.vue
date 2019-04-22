<template>
    <section class="container">
        <section class="section">
            <h1 class="title">
                Thank you for the feedback!
            </h1>
        </section>
    </section>
</template>

<script>
export default {
    created (){
      setTimeout( () => this.$router.push({ path: '/'}), 3000);
    }
}
</script>

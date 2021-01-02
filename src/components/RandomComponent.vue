<template>
  <div>
    <h1>somewords here</h1>
    <h2>{{ word }}</h2>
    <div class="box"></div>
  </div>
</template>

<script>
export default {
    name: "RandomComponent",
    props: {
        word: String
    }
}
</script>

<style scoped>
    @keyframes spin {
        0% { transform: rotate(20deg); background: green; margin-left: 20px; }
        20% { transform: rotate(30deg); background: red; margin-left: 50px;  }
        50% { transform: rotate(50deg); background: rgb(128, 0, 100); margin-left: 80px;}
        80% { transform: rotate(80deg); background: rgb(21, 42, 224); margin-left: 200px;}
        100% { transform: rotate(380deg); background: rgb(255, 212, 69); margin-left: 500px;}

    }
    .box {
        margin-top: 100px;
        background: green;
        width: 300px;
        height: 300px;
        display: block;
        animation: spin 4s infinite ease-in-out forwards;
        animation-direction: alternate;

    }
</style>
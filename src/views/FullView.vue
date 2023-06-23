<template>
    <header class="header">
        <slot name="header"></slot>
    </header>
    <main>
        <slot name="main"></slot>
    </main>
    <footer>
        <slot name="footer"></slot>
    </footer>
</template>

<script>
    export default{
        name: 'FullView'
    }
</script>

<style>
    .header{
        background-color: #333;
        color: #fff;
        padding: 40px 0px;
        text-align: center;
    }
    .main{
        background-color: #fff;
        color: #333;
        padding: 40px 0px;
        text-align: center;
    }
    .footer{
        background-color: #333;
        color: #fff;
        padding: 40px 0px;
        text-align: center;
    }
</style>
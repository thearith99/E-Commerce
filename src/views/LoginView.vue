<template>
    <body>
        <div class="form">
            <form>
                <label class="label">Email</label><br>
                <input type="text" placeholder="Enter Email" class="input"><br>
                <label class="label">Password</label><br>
                <input type="text" placeholder="Password" class="input"><br>
                <input type="checkbox">
                <label >Show</label>
                <RouterLink to="/register" class="register">Create</RouterLink><br>
                <button type="submit">Login</button>
            </form>
        </div>
    </body>
</template>


<script>
    
    
</script>


<style scoped>
    body{
        width: 50%;
        height: 400px;
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
        margin: 0px auto;
    }
    .form{
        width: 100%;
        height: 100%;
        padding: 100px;
    }
    .label{
        font-family: 'Rajdhani', sans-serif;
        font-size: 20px;
        font-weight: bold;
        margin-top: 5px;
    }
    label{
        font-family: 'Rajdhani', sans-serif;
        font-size: 15px;
        font-weight: bold;
    }
    .input{
        width: 500px;
        height: 30px;
        border-radius: 5px;
        border: 2px solid grey;
        margin-top: 5px;
    }
    button{
        width: 80px;
        height: 30px;
        margin: 30px 200px;
    }
    .register{
        text-decoration: none;
        font-family: 'Rajdhani', sans-serif;
        font-size: 15px;
        font-weight: bold;
        color: rgb(47, 43, 43);
        padding-left: 20px;
    }
</style>
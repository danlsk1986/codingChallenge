<template>
    <div class="header">
        <img id="logo" src="../assets/aerolab-logo.svg" alt="aerolabLogo">
        <div class="userInfo">
            <div class="userName">John Kite</div>
            <div class="userPoints">6000
              <img id="coin" src="../assets/icons/coin.svg" alt="coinIcon">  
            </div>
        </div>
    </div>
</template>

<script>

const user = 'https://coding-challenge-api.aerolab.co/user/me';
let token= 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJfaWQiOiI1ZDFhNGI0YWVhOTI1NTAwN2E2Yjk0OGYiLCJpYXQiOjE1NjIwMDQyOTh9.gUz9KOL99r9n3DjBhRrwoqtX10W03GxjbzL0SdacaCA'


fetch(user, {
    method: 'GET',
    headers: {
        'Authorization': token
    }
})
.then(response => response.json())
.then(data=> console.log(data))

export default {
    name: 'HeaderComponent'
}
</script>
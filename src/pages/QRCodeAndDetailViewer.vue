<template>
    <!-- you define your Vue template here -->
    <div class="card-container">
        <div class="card">
            <div>
                <q-img src="../images/image-qr-code.png" basic />
            </div>
            <div>
                <h5>Improve your front-end skills by building projects</h5>
            </div>
            <div>
                <p>Scan the QR code to visit Frontend Mentor and take your codeing skills to the next level</p>
            </div>
        </div>
    </div>
</template>
  
<script>
// This is where your Javascript goes
// to define your Vue component, which
// can be a Layout, a Page or your own
// component used throughout the app.
// import { defineComponent } from 'vue'
import { defineComponent } from 'vue'
import { QImg } from 'quasar' // Import QImg from Quasar

export default defineComponent({
    components: {
        QImg, // Register QImg component
    },
})
</script>
  
<style>
/* This is where your CSS goes */
p {
    font-size: 15px;
    font-weight: 400;
    text-align: center;
    color: hsl(220, 15%, 55%);
}

h5 {
    font-weight: 700;
    text-align: center;
    font-size: 20px;
    margin: 20px auto 10px;
    color: hsl(218, 44%, 22%);
}

@media screen and (max-width: 1440px) {
    .card {
        width: 30%;
        border-radius: 5px;
        padding: 20px;
        background-color: white;
        margin: auto;
    }

    .card-container {
        background-color: hsl(212, 45%, 89%);
        padding: 100px;
        /* margin-top: 100px; */
    }
}

@media screen and (max-width: 375px) {
    .card {
        width: 80%;
        border-radius: 13px;
        padding: 15px;
        background-color: hsl(0, 0%, 100%);
        margin: auto;
    }

    .card-container {
        background-color: hsl(212, 45%, 89%);
        padding: 70px 20px;
        margin-top: 0px;
        height: 100vh;
    }
}
</style>
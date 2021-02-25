<template>
    <div class="home-section">
        <div class="section-content">
          <div class="intro">
            <h1>I am a Fullstack Dev.</h1>
            <p>Jack of all trades, master of none.</p>
          </div>
        </div>
        <div class="btn">
            <button>Explore</button>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Home'
}
</script>

<style scoped>
    .home-section {
        grid-column-start: 2;
        grid-column-end: 3;
        display: grid;
        grid-template-rows: 1fr 30px;
        background-image: url("../assets/clip-waiting.png");
        background-size: cover;
    }

    .section-content {
        display: flex;
        flex-direction: row;
        grid-row: 1/2;
    }

    .btn {
        grid-row-start: 2;
        grid-row-end: 4;
        grid-column-start: 1;
        grid-column-end: 2;
    }

    .btn button {
        border: none;
        background: none;
        border: 1px solid var(--secondary);
        padding: 6px 16px;
        color: white;
        font-size: 0.6rem;
        outline: none;
        cursor: pointer;
    }

    .intro {
        display: flex;
        flex-wrap: wrap;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }
    
    .intro h1 {
        font-size: 2rem;
        color: var(--secondary);
    }

    .intro p {
        font-size: 0.6rem;
        font-weight: 100;
        color: grey;
    }

    .svg-image {
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
        height: 50px;
        width: 50px;
    }

    .svg-image img {
        position: relative;
        background-size: cover;
    }

    
</style>
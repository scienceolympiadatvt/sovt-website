commenting out the script did make the white screen go away :



<svelte:head>
    <title>Science Olympiad at Virginia Tech</title>
    <meta name="description" content="Science Olympiad at Virginia Tech is a student-run 
    organization at VT that hosts Science Olympiad tournaments and pursues outreach to 
    underdeveloped schools in STEM. Our 2024 Invitational will be held on January, 27, 2024.">
</svelte:head>

<script>
    import Button from '$lib/Button.svelte';
</script>

<div class='bg-image'></div>

<div class="content">
    <img src="/images/sovtlogo_transparent_white.png" class="big-logo" alt="Main SO@VT Logo">

    <div class="border b"></div>
    <div class="border"></div>

    <div class="invy-banner">
        Division C Invitational
        <br>
        <p style="font-size:medium; margin-top: 0.25rem;"></p>

        <b>January 30, 2027</b>
        <br><br>
        <Button
            text="Tournament Info"
            url="/tournament-info"
            bgcolor="#FF5EC9"
            txtcolor="black"
            active={true}
        />
    </div>
</div>


<style>

    .bg-image {
        /* The image used */
        background-image: url("/images/galaxy.jpg");


        /* Full height */
        /* height: 100vh;
        width: 100vw; */
        min-height: 100vh;
        min-width: 100vw;
        position:fixed;
        top:0;
        left:0;

        /* Center and scale the image nicely */
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        /* background-repeat: no-repeat;
        background-attachment: fixed;
        background-size: cover; */
    }

    /* :global(body) {
        margin: 0;
        height: 100vh;

        overflow: hidden;
    } */


    .content {

        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        position: absolute;
        top: 50%;
        left: 45%;
        transform: translate(-50%, -50%);
        width: 90vw;

    }

    .big-logo {

        width: 30rem;
        padding: 5rem;
    }

    .border {
        width: 1rem;

        height: 30rem;

    }

    .border.b {
        border-right: 5px solid #FF5EC9;
        animation: growHeight ease 2s 1 forwards;
    }

    .invy-banner {

        text-align: center;
        font-size: 2rem;
        font-family: 'Montserrat', sans-serif;
        color: white;

        padding: 7rem;
        animation: fadeInAnimation ease 2s 1 forwards;

    }

    @keyframes growHeight {
        0% {
            height: 0;
        }
        100% {
            height: 30rem;
        }
    }

    @keyframes growWidth {
        0% {
            width: 0;
        }
        100% {
            width: 15rem;
        }
    }

    @keyframes fadeInAnimation {
        0% {
            opacity: 0;
        }
        100% {
            opacity: 1;
        }
    }

    @media (max-width: 1000px) {
        .content {
            margin-top: 4rem;
            flex-direction: column;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
        }

        .border {
            width: 15rem;
            height: 1rem;
        }

        .big-logo {
            width: 20rem;
            padding: 0rem;
        }

        .invy-banner {
            padding: 3rem;
            font-size: 1.5rem;
        }

        .border.b {
            border-bottom: 5px solid #B8860B;
            border-right: 0px solid #B8860B;
            animation: growWidth ease 2s 1 forwards;
        }
    }

</style>

heres my page.svelte code

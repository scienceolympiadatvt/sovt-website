<svelte:head>
    <title>Past Tournaments</title>
</svelte:head>

<script>
    import Button from '$lib/Button.svelte';
</script>

<div class="bg-image"></div>

<div class="content">
    <div class="title">
        Past Tournaments
    </div>
    <br>

    <div class="section">
        <h2>
            2026 Division C Invitational
        </h2>
    
        <p style="">
            Despite it being online, we hope you enjoyed our virtual tournament!
        </p>

        <Button text="Results" url="https://www.duosmium.org/results/2026-02-04_virginia_tech_invitational_c/" active={true}/>
        <br>
        <Button text="Tests" url="https://drive.google.com/drive/folders/1ZJfC7IBFYWdL6u1_AsnJjA3KU2XMeN5V?usp=sharing" active={true}/>
    </div>

    <div class="section">
        <h2>
            2025 Division C Invitational
        </h2>
    
        <p style="">
            Congrats to all the teams who participated! We also hope you enjoyed our new trial events, Hokie Hunt and Disney Trivia.
        </p>

        <Button text="Results" url="https://www.duosmium.org/results/2025-02-01_virginia_tech_invitational_c/" active={true}/>
        <br>
        <Button text="Tests" url="https://drive.google.com/drive/folders/1uv_aNdDVI8ZS1jmfVil6X9VnU3MyuS55?usp=sharing" active={true}/>
    </div>


    <div class="section">
        <h2>
            2024 Division C Regional
        </h2>
    
        <p style="">
            Official Virginia Regional tournament, ran with VASO and feat. The Hokie Bird!
        </p>

        <Button text="Results" url="https://www.duosmium.org/results/2024-02-17_VA_virginia_tech_regional_c/"/>
        <br>
    </div>

        
    <div class="section">
        <h2>
            2024 Division C Invitational
        </h2>
    
        <p style="">
            Our first in-person tournament in 4 years! Thanks to all the volunteers, coaches, teams, and staff who helped make this possible. 
        </p>

        <Button text="Results" url="https://www.duosmium.org/results/2024-01-27_virginia_tech_invitational_c/"/>
        <br>
        <Button text="Tests" url="https://drive.google.com/drive/folders/1QXQGpW1TwGaJTJ470ITslaKDNzSRF1-V?usp=drive_link"/>
    </div>

    <div class="section">
        <h2>
            2023 Division B Invitational
        </h2>
    
        <p style="">
            Congrats to all the teams who participated in this online invitational!
        </p>

        <Button text="Results" url="https://www.duosmium.org/results/2023-01-21_virginia_tech_invitational_b/"/>
        <br>
        <Button text="Tests" url="https://drive.google.com/drive/folders/10YtifYp5YcgQuSouOcCOTaI0lU9HrNus?usp=sharing"/>

    </div>

</div>



<style>

    * {
        font-family: 'Montserrat', sans-serif;
    }

    .bg-image {
        /* The image used */
        background-image: url("/");
        z-index: -1;
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

    .title {
        text-align: center;
        font-size: 3rem;

    }
    .content {

        width: 75vw;

        padding: 3rem;

        background-color: rgba(255, 255, 255, 0.9);
        border-radius: 5rem;

        text-align: center;
        font-size: 1rem;
        margin-top: 10rem;
        margin-left: auto;
        margin-right: auto;
    }

    .section {
        margin-top: 3rem;
        text-align: center;
        margin-left: auto;
        margin-right: auto;
    }

    .section:hover h2::after{
        width: 30rem;
        background-color: rgba(106, 44, 62);
    }

    h2 {
        position: relative;
    }

    h2::after {
        content: "";
        height: 3px;
        width: 10rem;
        max-width: 50vw;
        background-color: orange;
        position: absolute;
        bottom: -.5em; 
        left: 50%;
        transform: translate(-50%);

        transition: 0.3s;
    }


</style>






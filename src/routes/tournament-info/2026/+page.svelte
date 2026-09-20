<svelte:head>
    <title>Tournament Info</title>
</svelte:head>
<script>
    import Card from '$lib/Card.svelte'; 
    import Button from '$lib/Button.svelte';
</script>

<div class='bg-image'></div>
<div class="content">
    <div class="title">
        <b>2026 Virginia Tech Invitational</b>
    </div>

    <br>
    
    <div class="cards">
        <Card title="Date" content="1/31/26"/>
        <Card title="Division" content="C"/>
        <Card title="Team # Cap" content="32"/>
        <Card title="Cost" content="$125"/>
    </div>
    
    <div class="info">
        <b>We're excited to announce the 2026 Virginia Tech Invitational! 
            It will be held on Virginia Tech's campus in Blacksburg, Virginia 
            and is open to teams from Virginia and across the country.</b>
    

        <div class="section">
            <h2>
                Registration
            </h2>
            <br>
            <p style="text-align:center; width:75%; margin:auto">
                Registration cost will be <b>$125</b> for all teams, up to a maximum of 3 teams per school. 
                Our team cap this year is 32 teams. Registration is first come, first serve, and will open on 
                <b>September 22</b> for all teams. In the case of capacity, Virginia teams will be given priority off the waitlist.
                <br><br>
            </p>
    
            <p style="text-align:center; width:75%; margin:auto">
                We welcome both veteran and new teams to gain competition experience at our tournament. If you are a Virginia school 
                and qualify for the VASO Outreach Initiative, the registration fee will instead be $65. 
                If your school otherwise has special circumstances that prevent you from paying the registration fees, 
                please reach out to us at scienceolympiadvt@gmail.com
        
                <br><br>
                <Button text="Register Here" url="https://docs.google.com/forms/d/e/1FAIpQLSfIJPr-Qsn3Vzu81WvKvHpUXE2WlsvyCE-NhNRDihZq_-7uoA/viewform" active={false}/>
        
                <b style="font-size:.75rem;">Registration closed November 7</b>
        
            </p>
        </div>

        <div class="section">

            <h2>Why SO@VT?</h2>

            <h1 class="subtitle" style="text-decoration-color: darkorange;">Explore Virginia Tech</h1>
            <p style='text-align:left'>We will have opportunities for exclusive university lab tours, 
                connecting with VT students and programs, and meeting the Hokie 
                Bird (our wonderful school mascot!). We encourage students to 
                explore VT’s campus and award-winning dining halls during our 
                tournament.</p>

                <br>

            <h1 class="subtitle" style="text-decoration-color: darkorange;">Build Events</h1>
            <p style='text-align:left'>We’re working closely with VASO to align 
                build testing with Regionals and State tournament standards. 
                We expect to run all builds this year.</p>

                <br>

            <h1 class="subtitle" style="text-decoration-color: darkorange;">Test Events</h1>
            <p style='text-align:left'>Our writers are experienced Science Olympiad 
                alumni from Virginia Tech and other colleges. 
                Tests go through rounds of thorough review and revision to ensure quality.</p>

                <br>

            <h1 class="subtitle" style="text-decoration-color: darkorange;">Early-Spring Regionals Prep</h1>
            <p style='text-align:left'>We are targeting our invitational to give teams the
                 best competitive start to the Regionals/States season. 
                 Virginia teams can return for our Virginia Tech Regional 
                 on February 21st, 2026.</p>

            
                 <br>

            <h1 class="subtitle" style="text-decoration-color: darkorange;">Webinars and Support</h1>
            <p style='text-align:left'>We host an annual Q&A webinar leading up 
                to our competition, where SO alumni give competition advice. 
                We’d love to answer any questions you have about our tournament 
                or team logistics in general.</p>

            <!-- <h2>
                Tests
            </h2>
        
            <p>
                Tournament quality is extremely important to us. Tests will be written by experienced Science Olympiad alumni from Virginia Tech and around the country. 
                Each test goes through a series of checks and deadlines to ensure the highest quality. <br>
                <br>
            </p> -->
        </div>

        <div class="section">
            <h2>
                Campus Map, Food, Schedule, VT Programs
            </h2>
        
            <p>
                Coming Soon! 🦃
        
            </p>
        </div>


    </div>
</div>



<style>

    .title {
        text-align: center;
        font-family: 'Montserrat', sans-serif;
        font-size: 3rem;

    }

    .division {
        text-align: center;
        font-family: 'Montserrat', sans-serif;
        font-size: 1.5rem;
        font-style: italic;
    }

    .cards {
        display: flex;
        align-items: center;
        justify-content: center;
        margin-top: 2rem;
    }

    .info {

        margin-left: auto;
        margin-right: auto;
        margin-top: 2rem;
        text-align: center;
        font-family: 'Montserrat', sans-serif;
        font-size: 1rem;
    }

    .section {
        margin-top: 3rem;
        text-align: center;
        margin-left: auto;
        margin-right: auto;
    }

    .content {

        background-color: rgba(255, 255, 255, .9);
        margin-top: 8rem;
        width: 70vw;
        text-align: center;
        margin-left: auto;
        margin-right: auto;

        border-radius: 5rem;

        padding: 3rem;
    }

    .bg-image {
        /* The image used */
        background-image: url("/images/dark_blueish_blur.jpg");
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
        max-width: 75vw;
        background-color: orange;
        position: absolute;
        bottom: -.5em; 
        left: 50%;
        transform: translate(-50%);

        transition: 0.3s;
    }


    .subtitle {

        font-size: 1.15rem;
        font-weight: 1000;
        text-decoration: underline;
        text-underline-offset: .4rem;
        /* text-decoration-color: orange; */
        text-align: left;

    }


    @media (max-width: 1000px) {
        .cards {
            display: none;
        }   

        .division {
            display: inline;
        }   
    }



</style>

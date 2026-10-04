<svelte:head>
    <title>About Us</title>
</svelte:head>

<script>
    import Button from '$lib/Button.svelte';
</script>

<div class="bg-image"></div>

<div class="content">
    <div class="title">
        About Us
    </div>
    <br>
    We are a group of 3,859 officers and over 100 student volunteers, who have operated since 2018. 

    <div class="section">
        <h2>Exec</h2>
        <div class="officer-container">
            <div class="officer">
                <img src="images/photoshoot/jake.jpg" alt="Jake Smith" style="border: 5px solid #076c9b;">
                <p>Jake O' Brien</p>
            </div>
            <div class="officer">
                <img src="images/photoshoot/josh.jpg" alt="Josh Gao" style="border: 5px solid #076c9b;">
                <p>Josh Gao</p>
            </div>
            <div class="officer">
                <img src="images/photoshoot/thiviya.jpg" alt="Thiviya Kumar" style="border: 5px solid #076c9b;">
                <p>Thiviya Karuppasamy</p>
            </div>
            <div class="officer break"></div>
            <div class="officer">
                <img src="images/photoshoot/joylyn.jpg" alt="Joylyn Wang" style="border: 5px solid #076c9b;">
                <p>Joylyn Wang the GOAT</p>
            </div>
            <div class="officer">
                <img src="images/photoshoot/vy.jpg" alt="Vy Tran" style="border: 5px solid #076c9b;">
                <p>Vy Nguyen</p>
            </div>
        </div>
    </div>

    <div class="section">
        <h2>Tournament Logistics</h2>
        <div class="officer-container">
            <div class="officer">
                <img src="images/photoshoot/sanjay.jpg" alt="SO@VT Team" style="border: 5px solid #8e3108;">
                <p>Sanjay Shankar</p>
            </div>
            <div class="officer">
                <img src="images/photoshoot/orion.jpg" alt="SO@VT Team" style="border: 5px solid #8e3108;">
                <p>Orion Keller</p>
            </div>
            <div class="officer">
                <img src="images/photoshoot/reagan.jpg" alt="SO@VT Team" style="border: 5px solid #8e3108;">
                <p>Reagan Nguyen</p>
            </div>
            <div class="officer break"></div>
            <div class="officer">
                <img src="images/photoshoot/tarun.jpg" alt="SO@VT Team" style="border: 5px solid #8e3108;">
                <p>Tarun Nandamudi</p>
            </div>
            <div class="officer">
                <img src="images/photoshoot/catherine.jpg" alt="SO@VT Team" style="border: 5px solid #8e3108;">
                <p>Catherine Felix</p>
            </div>
        </div>
    </div>

    <div class="section">
        <h2>Volunteering</h2>
        <div class="officer-container">
            <div class="officer">
                <img src="images/photoshoot/devyn.jpg" alt="SO@VT Team" style="border: 5px solid #e7a8e0;">
                <p>Devyn Hopkins</p>
            </div>
            <div class="officer">
                <img src="images/photoshoot/sanjana.jpg" alt="SO@VT Team" style="border: 5px solid #e7a8e0;">
                <p>Sanjana Rayani</p>
            </div>
        </div>
    </div>

    <div class="section">
        <h2>Outreach</h2>
        <div class="officer-container">
            <div class="officer">
                <img src="images/photoshoot/lauren.jpg" alt="SO@VT Team" style="border: 5px solid #e40000;">
                <p>Lauren Spehlmann</p>
            </div>
            <div class="officer">
                <img src="images/photoshoot/caroline.jpg" alt="SO@VT Team" style="border: 5px solid #e40000;">
                <p>Caroline Shoop</p>
            </div>
            <div class="officer">
                <img src="images/photoshoot/simba.jpeg" alt="SO@VT Team" style="border: 5px solid #e40000;">
                <p>Simba Srivastava</p>
            </div>
        </div>
    </div>

    <div class="section">
        <h2>Public Relations</h2>
        <div class="officer-container">
            <div class="officer">
                <img src="images/photoshoot/vicky.jpg" alt="SO@VT Team" style="border: 5px solid #6cbe68;">
                <p>Victoria Fedik</p>
            </div>
            <div class="officer">
                <img src="images/photoshoot/sarayu.jpg" alt="SO@VT Team" style="border: 5px solid #6cbe68;">
                <p>Sarayu Pulipati</p>
            </div>
            <div class="officer">
                <img src="images/photoshoot/arushi.jpg" alt="SO@VT Team" style="border: 5px solid #6cbe68;">
                <p>Arushi Deb</p>
            </div>
        </div>
    </div>

    <br><br>
    <p>Our <b>mission</b> is to foster competitive Science Olympiad in the heart of Southwest Virginia, 
        leading to life-changing STEM experiences. We do so through two priorities:</p>
    <br>
    <div class="emphasis"><span>Hosting high-quality tournaments,</span> facilitated by dedicated Virginia Tech students in STEM</div>
    <br>
    
    <div class="emphasis"><span>Pursuing outreach initiatives</span> to schools and new teams, locally and online</div>

    <br>

    <br>

    We welcome you to connect with us! Please see our <a href="/contact" class="button">Contact</a> page.

</div>



<style>

    * {
        font-family: 'Montserrat', sans-serif;
    }

    .bg-image {
        /* The image used */
        background-image: url("/images/fall_burruss.jpg");
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

        width: 70vw;

        padding: 3rem;

        background-color: rgba(255, 255, 255, 0.9);
        border-radius: 5rem;

        text-align: center;
        font-size: 1rem;
        margin-top: 10rem;
        margin-left: auto;
        margin-right: auto;
    }

    .emphasis {
        font-size: 1.5rem;
    }

    span {
        color: rgb(255, 102, 0);
    }

    img {
        width:250px;
        max-width: 75vw;
        margin-right: 1rem;
        margin-bottom: 1rem;
        margin-top: 1rem;
        margin-left: 1rem;
        /* margin-left: auto;
        margin-right: auto; */
        /* display: block; */
    }

    .officer-container {
        display: flex; /* Enables Flexbox layout */
        flex-wrap: wrap; /* Allows items to wrap to the next row */
        justify-content: center; /* Centers the officer blocks horizontally */
        gap: 10px; /* Adds uniform spacing between officer blocks */
        margin: 0px 0; /* Optional: Add spacing around the container */
    }

    .officer {
        display: flex;
        flex-direction: column; /* Stack image and text vertically */
        align-items: center; /* Ensure the image and text are centered */
        text-align: center; /* Center-align text inside the block */
        width: 250px; /* Ensure uniform width for all officer blocks */
    }

    .officer.break {
        flex-basis: 100%; /* Force this item to take a full row */
        max-width: 100%; /* Ensure it spans the full width */
    }


    .officer img {
        /* width:200px;
        max-width: 75vw; */
        margin-right: 1rem;
        margin-bottom: 0rem;
        margin-top: 0rem;
        margin-left: 1rem;
        width: 100%; /* Ensure image fits within the officer block */
        max-width: 200px; /* Set max width to match the officer block width */
        height: auto; /* Maintain aspect ratio */
        border-radius: 10px; /* Optional: Add rounded corners */
    }

    .officer p {
        margin: 10px 0 0; /* Add spacing above the text */
        font-size: 18px; /* Set font size */
        width: 100%; /* Match text width to the officer block */
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

# my-presentation
Website for my hackathon presentation
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ICT & HUMSS Celebration Week Event</title>
    <style>
             
             /* === General Body and Background Styles === */
body {
    background-color: #212730; /* Dark grey background */
    color: #ffffff; /* White text */
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 0;
    position: relative;
}

/* === Gradient Overlay (Background Effect) === */
.color-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: linear-gradient(135deg, rgb(15, 62, 120), #434f5ce5); /* Black to Light Blue */
    z-index: -1; /* Para hindi matakpan ang ibang content */
}

/* === Header Styles === */
header {
    display: flex;
    justify-content: space-between; /* Pagkaayos ng mga items sa header */
    align-items: center;
    padding: 30px 40px;
    border-top: 2px solid #00aaff;
    border-bottom: 3px solid #00aaff;
    background-color: #242e32;
}

/* Logo Styles */
.logo {
    display: flex;
    align-items: center;
    font-size: 32px;
    font-weight: bold;
    color: #00aaff; /* Light Blue */
    letter-spacing: 2px;
    text-transform: uppercase;
    transition: color 0.3s ease; /* Para magbago ang kulay kapag nag-hover */
}
.logo:hover {
    color: #53c3ff; /* Lighter Blue */
    text-shadow: 2px 2px 5px rgba(9, 136, 255, 0.72); /* Shadow effect */
}

.logo-img {
    width: 40px;
    height: auto;
    margin-right: 15px;
    border-radius: 10px; /* Round ang mga corner ng logo */
}

/* Navbar Styles */
.navbar {
    display: flex;
    gap: 30px; /* Distance between navbar items */
    font-size: 18px;
    font-weight: bold;
}

.navbar a {
    color: #ffffff; /* White text color */
    text-decoration: none; /* Walang underline */
    transition: color 0.3s ease, transform 0.3s ease;
}

.navbar a:hover {
    color: #00aaff; /* Light Blue color sa hover */
    transform: translateY(-5px); /* Tumatalon ng kaunti kapag nag-hover */
}

.navbar a.active {
    color: #00aaff; /* Light Blue color sa active state */
    text-decoration: underline;
}

/* Contact Link Styles */
.contact {
    color: #ffffff;
    font-size: 18px;
    text-decoration: none;
    padding: 10px 15px;
    border: 2px solid #00aaff; /* Light Blue border */
    border-radius: 5px;
    transition: all 0.3s ease;
}

.contact:hover {
    color: #212730; /* Dark Grey text */
    background-color: #00aaff; /* Light Blue background */
    border-color: #00aaff;
}

/* === Home Section === */
.Home {
    display: flex;
    justify-content: space-between;
    padding: 10% 8%;
    align-items: center;
    flex-wrap: wrap;
    position: relative;
}

#background-video {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    z-index: -1;
    opacity: 0.7; /* Para di masyadong makapal ang video sa background */
}

.H-content h1 {
    font-size: 70px;
    color: #00aaff; /* Light Blue */
    margin-bottom: 10px;

}


.H-content p {
    font-size: 20px;
    color: #ffffff; /* White */
}

/* === Image Box Styling === */
.img-box img {
    border-radius: 50%; /* Round Image */
    width: 600px;
    height: 500px;
    box-shadow: 0 10px 20px rgb(173, 216, 230); /* Light Blue shadow */
}

/* === About Section === */
.about {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 12% 8%;
    gap: 5em;
    background: #212730; /* Dark Grey with transparency */
    border-top: 2px solid #00aaff; /* Light Blue border */
}

.about-img img {
    width: 500px;
    border-radius: 10%; /* Slightly rounded corners */
    box-shadow: 0 10px 20px rgb(173, 216, 230); /* Light Blue shadow */
}

.about-content h2, .about-content h3 {
    color: #ffffff; /* White text */
    margin: 0;
}

.about-content h2 {
    font-size: 40px;
}

.about-content h3 {
    font-size: 50px;
}

.about-content p {
    color: #ffffff;
    font-size: 18px;
    margin: 1.5em 0;
}

/* Discover button styling */
.discover-box-wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;
}

.discover-box-content {
    background-color: #00aaff; /* Light Blue */
    color: #ffffff; /* Black text */
    padding: 10px 20px;
    font-size: 18px;
    font-weight: bold;
    text-align: center;
    border-radius: 8px;
    text-decoration: none;
    transition: background-color 0.3s, transform 0.3s;
}

.discover-box-content:hover {
    background-color: #0099cc; /* Slightly darker Light Blue */
    transform: scale(1.05); /* Para mag-zoom in kapag nag-hover */
}

/* === Footer Styling === */
footer {
    background-color: #212730; /* Dark Grey */
    padding: 20px 0;
    text-align: center;
    color: #212121; /* White text */
    border-top: 3px solid #00aaff; /* Light Blue border */
}

.footer-content {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
    align-items: center;
}

.footer-item {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
}

.footer-item a {
    color: #00aaff; /* Light Blue */
    font-size: 16px;
    text-decoration: none;
    transition: color 0.3s ease, transform 0.3s ease;
}

.footer-item a:hover {
    color: #ffffff; /* White */
    transform: scale(1.1); /* Zoom in effect sa hover */
}

footer img {
    width: 30px;
    height: auto;
    transition: transform 0.3s ease;
}

footer img:hover {
    transform: scale(1.2); /* Zoom in effect sa mga icons sa footer */
}

footer p {
    margin-top: 12px;
    font-size: 14px;
    color: #d9d9d9; /* Light grey color */
}

/* === Second Footer Styling === */
.footer-2nd {
    background-color: #0c1c21; /* Darker Grey */
    padding: 15px 0;
    text-align: center;
    color: #212730; /* White text */
    border-top: 3px solid #00aaff; /* Light Blue border */
    font-size: 14px;
}

.footer-2nd .footer-content {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 10px;
    max-width: 1200px;
    margin: 0 auto;
}

/* === Media Queries for Responsiveness === */
@media screen and (max-width: 768px) {
    /* Header Layout Adjustments */
    header {
        padding: 10px 5px; /* Reduced padding for better fit */
        flex-direction: column; /* Stack logo and nav vertically */
        text-align: center;
    }

    /* Logo adjustments for small screens */
    .logo {
        font-size: 22px; /* Smaller font size for the logo */
    }

    .logo-img {
        width: 28px; /* Slightly smaller logo image */
        margin-right: 8px; /* Reduced margin */
    }

    /* Navbar Links Adjustments */
    .navbar {
        flex-direction: column; /* Stack navbar items vertically */
        gap: 12px; /* Reduced gap between links */
        margin-top: 15px;
    }

    .navbar a {
        font-size: 14px; /* Smaller font size for navbar links */
    }

    .navbar a.active {
        font-size: 15px; /* Active link slightly larger for emphasis */
    }

    /* Home Section Adjustments */
    .Home {
        padding: 5% 3%; /* Adjusted padding for mobile view */
        text-align: center;
    }

    .Home h1 {
        font-size: 36px; /* Smaller heading size for mobile */
    }

    .H-content p {
        font-size: 14px; /* Smaller font size for mobile text */
        margin-top: 10px;
    }

    /* Image Box adjustments for smaller screens */
    .img-box img {
        width: 90%; /* Make image slightly smaller for mobile */
        height: auto;
        max-width: 100%;
    }

    /* About Section Adjustments */
    .about {
        padding: 8% 4%; /* Adjusted padding for mobile */
        flex-direction: column; /* Stack content vertically */
        text-align: center;
    }

    .about-img img {
        width: 70%; /* Smaller image for mobile view */
        margin-bottom: 20px;
    }

    .about-content h2 {
        font-size: 28px; /* Slightly smaller subheading */
    }

    .about-content h3 {
        font-size: 30px; /* Slightly smaller subheading for mobile */
    }

    .about-content p {
        font-size: 15px; /* Adjusted font size for better readability */
        margin: 1em 0;
    }

    /* Discover Button Adjustments */
    .discover-box-wrapper {
        width: 100%; /* Full width button */
        margin-top: 15px; /* Adjusted spacing */
    }

    .discover-box-content {
        padding: 12px 20px; /* Slightly smaller padding for mobile */
        font-size: 16px; /* Adjusted font size for mobile */
        text-align: center;
    }

    /* Footer Adjustments */
    footer {
        padding: 12px 0; /* Adjusted padding for better mobile spacing */
    }

    .footer-content {
        flex-direction: column; /* Stack footer items vertically */
        gap: 12px;
    }

    .footer-item {
        flex-direction: column; /* Align icon and link vertically */
        align-items: center;
        gap: 8px;
    }

    .footer-item a {
        font-size: 14px; /* Slightly smaller text for mobile links */
    }

    footer img {
        width: 22px; /* Smaller footer icons */
    }

    footer p {
        font-size: 12px; /* Smaller footer text for mobile */
    }

    /* Second Footer Adjustments */
    .footer-2nd {
        padding: 10px 0; /* Adjusted padding for the second footer */
    }

    .footer-2nd .footer-content {
        gap: 6px;
        flex-direction: column;
        align-items: center;
    }

    /* === Welcome Heading Adjustments for Mobile === */
    .welcome-heading {
        font-size: 5rem; /* Smaller font size for mobile (80px) */
        text-align: center; /* Keep text centered */
    }
}




    </style>
</head>
<body>

    <div class="color-overlay"></div>

    <!-- Header -->
    <header>
        <div class="logo">
            <img src="/Users/Nuel/Desktop/IMG_20250120_234245.jpg" alt="Logo" class="logo-img" aria-label="Website Logo">
            <span>MSV Hub</span>
        </div>
        <nav class="navbar">
            <a href="#" class="active">Event =></a>
            <a href="#">Bench Yell</a>
            <a href="#">Teknomodelo</a>
            <a href="#">Hackathon</a>
        </nav>
        <a href="#" class="contact" aria-label="About Me">About Us</a>
    </header>

    <!-- Home Section -->
    <section class="Home">
        <video autoplay muted loop id="background-video" poster="path-to-fallback-image.jpg">
            <source src="/Users/Nuel/Desktop/HomeVid.mp4" type="video/mp4">
            <!-- Fallback message for browsers that do not support the video element -->
        </video>

        <div class="H-content">
            <h1 style="font-size: 110px; color: #f1f1f1;">Welcome</h1>
            <h1 class="blue-h1"> <!--We are <span>MSV</span><br>an ICT student<br>Grade-11 "Group-1"</h1>-->We are Group 1 
            <br>ICT Students</h1>
            <p>Exploring Information and Communication Technology</p>
        </div>
    
        <div class="img-box">
            <img src="/Users/Nuel/Desktop/f821b07f43fdf8d2812c1f841b9479c8.jpg" alt="Sample Image" aria-label="Sample Image for Welcome Section">
        </div>
    </section>
    
    

    <!-- About Section -->
    <section class="about">

        <div class="about-img">
            <img src="/Users/Nuel/Desktop/467832570_579468575073007_8094157829861763811_n.jpg" alt="Before Image" aria-label="Image of Hackathon">
        </div>

        <div class="about-content">
            <h2 class="heading">ICT <span style="color: #00aaff;">HUMSS</span></h2>
            <h3>Hack<Span style="color: #00aaff;">athon</Span></h3>
            <p>The <strong>hackathon</strong>, also known as a <strong>codefest</strong>, is an exciting event where developers, creators, and innovators gather to collaborate in creating innovative solutions. It is an opportunity for enthusiastic individuals to brainstorm, design, and implement creative projects within a limited time frame, promoting rapid development and problem-solving.</p>
            <p>Overall, a <strong>hackathon</strong> focuses on:</p>
            <ul>
                <li><strong>Learning</strong> through hands-on experience and discovering new technologies.</li>
                <li><strong>Collaboration</strong>, where participants work together to exchange ideas and build projects.</li>
                <li><strong>Innovation</strong>, where teams strive to create cutting-edge solutions with the potential to change the future.</li>
            </ul>
         <br>
         <br>
            <div class="discover-box-wrapper">
                 <a href="#" class="discover-box-content">
                    <span> Discover More</span>
                </a>
            </div>
        </div>

    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-content">

            <div class="footer-item">
                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/Facebook_f_logo_%282019%29.svg/1200px-Facebook_f_logo_%282019%29.svg.png" alt="Facebook Logo" aria-label="Facebook Logo">
                <a href="https://www.facebook.com/share/1D9hGa7qi4/" target="_blank" aria-label="Visit Facebook Page">SHS ICT & HUMSS Department</a>
            </div>


            <div class="footer-item">
                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/Facebook_f_logo_%282019%29.svg/1200px-Facebook_f_logo_%282019%29.svg.png" alt="Facebook Logo" aria-label="Facebook Logo">
                <a href="https://www.facebook.com/share/1DAUvGV3PL/" target="_blank" aria-label="Visit SPCC Facebook Page">SPCC Caloocan Grade School Department</a>
            </div>

            <!-- fb -->
            <div class="footer-item">
                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/Facebook_f_logo_%282019%29.svg/1200px-Facebook_f_logo_%282019%29.svg.png" alt="Facebook Logo">
                <a href="https://www.facebook.com/groups/icthumss2024/?ref=share&mibextid=NSMWBT" target="_blank">ICT & HUMSS S.Y.2024-2025</a>
            </div>

            <!-- SPCC youtube -->
            <div class="footer-item">
                <img src="https://upload.wikimedia.org/wikipedia/commons/4/42/YouTube_icon_%282013-2017%29.png" alt="YouTube Logo">
                <a href="https://www.youtube.com/@spcccaloocan_official" target="_blank">SPCC YouTube</a>
            </div>
         
            <!-- Instagram -->
            <div class="footer-item">
                <img src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Instagram_icon.png" alt="Instagram Logo">
                <a href="https://www.instagram.com/spcccaloocan_official/" target="_blank">SPCC Caloocan Instagram</a>
            </div>

             <!-- TikTok -->
<div class="footer-item">
    <img src="/Users/Nuel/Desktop/377222338_1035863667645881_7036772377622772959_n.png" alt="TikTok Logo">
    <a href="https://www.tiktok.com/@spcccaloocan_official" target="_blank">SPCC TikTok</a>
</div>

            <!-- SPCC Google -->
            <div class="footer-item">
                <img src="/Users/Nuel/Desktop/423147491_722185566709436_4718446549001651679_n.png" alt="SPCC Logo">
                <a href="https://spcc.edu.ph/" target="_blank">SPCC.edu.ph</a>
            </div>

        </div>
    </footer>

    <footer class="footer-2nd">
        <div class="footer-content">
            <p>&copy; 2025 11-ICT. All rights reserved.</p>
        </div>
    </footer>

</body>
</html>

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Personal Portfolio Website</title>
    
    <script src="https://kit.fontawesome.com/e674bba739.js" crossorigin="anonymous"></script>
</head>
<style>
    * {
    margin: 0;
    padding: 0;
    font-family: 'Poppins', sans-serif;
    box-sizing: border-box;
}

body {
    background: #080808;
    color: #fff;
}

#header {
    width: 100%;
    height: 100vh;
    background-image: url("C:/Users/test/Desktop/My Portfolio/—Pngtree—creative technology science fiction cyberpunk_9015394.png");
    background-size: 550px;
    background-position: center;
    background-repeat: no-repeat;
}


.container {
    padding: 10px 10%;
}

nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
}

.logo {
    width: 140px;
}

nav ul li {
    display: inline-block;
    list-style: none;
    margin: 10px 20px;
}

nav ul li a {
    color: #ff004f;
    text-decoration: none;
    font-size: 18px;
    position: relative;
}

nav ul li a::after {
    content: '';
    width: 0;
    height: 3px;
    background: #ff004f;
    position: absolute;
    left: 0;
    bottom: -6px;
    transition: 0.5s;
}

nav ul li a:hover::after {
    width: 100%;
}

.header-text {
    margin-top: 20%;
    font-size: 30px;
}

.header-text h1 {
    font-size: 60px;
    margin-top: 20px;
}

.header-text h1 span {
    color: #ff004f;
}

/* ----------ABOUT---------- */
#about {
    padding: 80px 0px;
    color: #ababab;
}

.row {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.about-col-1 {
    flex-basis: 35%;
}

.about-col-1 img {
    width: 100%;
    border-radius: 15px;
}

.about-col-2 {
    flex-basis: 60%;
}

.sub-title {
    font-size: 60px;
    font-weight: 600;
    color: #fff;
}

.tab-titles {
    display: flex;
    margin: 20px 0 40px;
}

.tab-links {
    margin-right: 50px;
    font-size: 18px;
    font-weight: 500;
    cursor: pointer;
    position: relative;
}

.tab-links::after {
    content: '';
    width: 0;
    height: 3px;
    background: #ff004f;
    position: absolute;
    left: 0;
    bottom: -8px;
    transition: 0.5s;
}

/* .tab-links:hover::after{
width: 100%;
} */
.tab-links.active-link::after {
    width: 50%;
}

.tab-contents ul li {
    list-style: none;
    margin: 10px 0;
}

.tab-contents ul li span {
    color: #b54768;
    font-size: 14px;
}

.tab-contents {
    display: none;
}

.tab-contents.active-tab {
    display: block;
}

/* ----------SERVICES---------- */
#services {
    padding: 30px 0;
}

.services-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 40px;
    margin-top: 50px;
}

.services-list div {
    background: #262626;
    padding: 40px;
    font-size: 15px;
    line-height: 30 px;
    font-weight: 300;
    border-radius: 10px;
    transition: background 0.5s, transform 0.5s;
}

.services-list div i {
    font-size: 50px;
    margin-bottom: 30px;
}

.services-list div h2 {
    font-size: 30px;
    font-weight: 500;
    margin-bottom: 15px;
}

.services-list div a {
    text-decoration: none;
    color: #fff;
    font-size: 14px;
    margin-top: 20px;
    display: inline-block;
}

.services-list div:hover {
    background: #ff004f;
    transform: translateY(-10px);
}

/* ----------PORTFOLIO---------- */
#portfolio {
    padding: 50px 0;
}

.work-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 40px;
    margin-top: 50px;
}

.work {
    border-radius: 10px;
    position: relative;
    overflow: hidden;
}

.work img {
    width: 100%;
    border-radius: 10px;
    display: block;
    transition: transform 0.5s;
}

.layer {
    width: 100%;
    height: 0;
    background: #ff004f;
    border-radius: 10px;
    position: absolute;
    left: 0;
    bottom: 0;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    padding: 0 40px;
    text-align: center;
    font-size: 16px;
    transition: height 0.5s;
}

.layer h2 {
    margin-bottom: 30px;
}

.layer a {
    margin-top: 30px;
    color: #080808;
    text-decoration: none;
    font-size: 18px;
    line-height: 60px;
    background: #fff;
    width: 60px;
    height: 60px;
    border-radius: 50%;
    text-align: center;
}

.work:hover img {
    transform: scale(1.1);
}

.work:hover .layer {
    height: 100%;
}

.btn {
    display: block;
    margin: 50px auto;
    width: fit-content;
    border: 1px solid #ff004f;
    padding: 14px 50px;
    border-radius: 6px;
    color: #fff;
    text-decoration: none;
    transition: background 0.75s;
}

.btn:hover {
    background: #ff004f;
}

/* ----------CONTACT---------- */
.contact-left {
    flex-basis: 35%;
}

.contact-right {
    flex-basis: 60%;
}

.contact-left p {
    margin-top: 30px;
}

.contact-left p i {
    color: #ff004f;
    margin-right: 15px;
    font-size: 25px;
}

.social-icons {
    margin-top: 30px;
}

.social-icons a {
    text-decoration: none;
    font-size: 30px;
    margin-right: 15px;
    color: #ababab;
    display: inline-block;
    transition: color 0.5s, transform 0.5s;
}

.social-icons a:hover {
    color: #ff004f;
    transform: translateY(-5px);
}

.btn.btn2 {
    display: inline-block
}

.btn.btn3 {
    background: #080808;
    margin-top: 30px;
    transition: background 0.5;

}

.btn.btn3:hover {
    background: #ff004f;
}

.contact-right form {
    width: 100%;
}

form input,
form textarea {
    width: 100%;
    border: 0;
    outline: none;
    background: #262626;
    padding: 15px;
    margin: 15px 0;
    color: #fff;
    font-size: 18px;
    border-radius: 6px;
}

.copyright {
    width: 100%;
    text-align: center;
    padding: 25px 0;
    background: #262626;
    font-weight: 300;
    margin-top: 20px;
}

.copyright i {
    color: #ff004f;
    transition: color 0.5s;
}

.copyright i:hover {
    color: #fff;
}

nav .fas {
    display: none;
}

/* ----------CSS FOR SMALL SCREEN---------- */
@media only screen and (max-width: 600px) {
    #header {
        background-image: url("C:/Users/test/Desktop/My Portfolio/—Pngtree—creative technology science fiction cyberpunk_9015394.png");
    }

    .header-text {
        margin-top: 100%;
        font-size: 16px;
    }

    .header-text h1 {
        font-size: 30px;
    }

    nav .fas {
        display: block;
        font-size: 25px;
    }

    nav ul {
        background: #b54768;
        position: fixed;
        top: 0;
        width: 200;
        right: 0;
        height: 100vh;
        padding-top: 50px;
    }

    nav ul li {
        display: block;
        margin: 25px;
    }

}

/* ----------CSS FOR SMALL SCREEN---------- */
@media only screen and (max-width: 600px) {

    /* Adjust the header image and text size for small screens */
    #header {
        background-image: url("C:/Users/test/Desktop/My Portfolio/—Pngtree—creative technology science fiction cyberpunk_9015394.png");
    }

    .header-text {
        margin-top: 100%;
        font-size: 16px;
    }

    .header-text h1 {
        font-size: 30px;
    }

    /* Show the navigation menu on small screens */
    nav ul {
        display: none;
    }

    nav .fas {
        display: block;
        font-size: 25px;
    }

    nav ul {
        background: #b54768;
        position: fixed;
        top: 0;
        width: 200px;
        /* Increased the width to accommodate the menu items */
        right: 0;
        height: 100vh;
        padding-top: 50px;
        transform: translateX(200px);
        /* Off-canvas menu, initially hidden */
        transition: transform 0.3s ease-in-out;
    }

    nav ul.show {
        transform: translateX(0);
        /* Show the menu when 'show' class is applied */
    }

    nav ul li {
        display: block;
        margin: 25px;
    }
}
</style>

<body>
    <div id="header">
        <div class="container">
            <nav>
                <img src="C:\Users\test\Desktop\My Portfolio\fca0f3ec795e459faa7d10de8f821d2c.png" class="logo"></img>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">About</a></li>
                    <li><a href="#">Services</a></li>
                    <li><a href="#">Portfolio</a></li>
                    <li><a href="#">Contact</a></li>
                    <i class="fas fa-times"></i>
                </ul>
                <i class="fas fa-bars"></i>
            </nav>
            <div class="header-text">
                <p>UI/UX Designer</p>
                <h1>Hi, I'm <span>Rehaan</span><br>Ashraf from India</h1>
            </div>
        </div>
    </div>
    <!-- ----------ABOUT---------- -->
    <div id="about">
        <div class="container">
            <div class="row">
                <div class="about-col-1">
                    <img src="C:\Users\test\Desktop\My Portfolio\Rehaan img.jpg">
                </div>
                <div class="about-col-2">
                    <h1 class="sub-title">About Me</h1>
                    <p>I'm Rehaan, a creative UI/UX Designer from India, specializing in web and app development. My passion lies in crafting user-friendly and visually appealing interfaces. With a strong background in design and development, I create seamless digital experiences that leave a lasting impact. I stay updated with the latest design trends and technologies to deliver exceptional results. Collaborative and dedicated, I aim to exceed client expectations and solve complex challenges. When not designing, I find inspiration in music and the great outdoors. Let's collaborate and turn your ideas into remarkable digital solutions. Contact me to create something extraordinary together!</p>
                    <div class="tab-titles">
                        <p class="tab-links active-link" onclick="openTab('skills')">Skills</p>
                        <p class="tab-links" onclick="openTab('experience')">Experience</p>
                        <p class="tab-links" onclick="openTab('education')">Education</p>
                    </div>
                    <div class="tab-contents active-tab" id="skills">
                        <ul>
                            <li><span>UI/UX</span><br>Designing Web/App interfaces</li>
                            <li><span>Web Development</span><br>Web app Development</li>
                            <li><span>App Development</span><br>Building Android/iOS apps</li>
                        </ul>
                    </div>
                    <div class="tab-contents" id="experience">
                        <ul>
                            <li><span>2022 - Current</span><br>UI/UX Design at Amrita Institute</li>
                            <li><span>2019-2021</span><br>Freelance UI Designer</li>
                            <li><span>2017-2019</span><br>Web Developer Intern - XYZ Web Agency</li>
                            <li><span>2017-2019</span><br>Started to learn UI/Ux design.</li>
                        </ul>
                    </div>
                    <div class="tab-contents" id="education">
                        <ul>
                            <li><span>2022</span><br>Bachelor of Science in Computer Science at Amrita</li>
                            <li><span>2021</span><br>Certification in UI/UX Design</li>
                            <li><span>2019</span><br>High School Diploma in Redbridge International</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- ----------SERVICES---------- -->
    <div id="services">
        <div class="container">
            <h1 class="sub-title">My Services</h1>
            <div class="services-list">
                <div>
                    <i class="fa-brands fa-android"></i>
                    <h2>App Development</h2>
                    <p>As an experienced app developer, I have a passion for creating innovative and user-friendly mobile applications. I specialize in building both Android and iOS apps that cater to diverse industries and user needs. My expertise includes the use of modern programming languages, frameworks, and design patterns to ensure seamless functionality and exceptional user experiences.</p>
                    <a href="#">Learn more</a>
                </div>
                <div>
                    <i class="fa-solid fa-code"></i>
                    <h2>Web Development</h2>
                    <p>With a strong background in web development, I craft dynamic and responsive websites that deliver an immersive online presence. I am proficient in front-end technologies such as HTML, CSS, and JavaScript, as well as back-end technologies like Node.js and PHP. My focus on performance optimization and cross-browser compatibility ensures a smooth user experience across various devices.</p>
                    <a href="#">Learn more</a>

                </div>
                <div>

                    <i class="fa-solid fa-crop-simple"></i>
                    <h2>UI/UX Design</h2>
                    <p>UI/UX design is at the heart of my creative process. I have a keen eye for aesthetics and usability, and I believe in putting users first. By conducting in-depth user research and creating intuitive wireframes, I design visually appealing interfaces that seamlessly guide users through their journey. I take pride in crafting delightful user experiences that leave a lasting impression.</p>
                    <a href="#">Learn more</a>
                </div>
            </div>
        </div>
    </div>
    <!-- ----------PORTFOLIO--------- -->
    <div id="portfolio">
        <div class="container">
            <h1 class="sub-title">My Works</h1>
            <div class="work-list">
                <div class="work">
                    <img src="C:\Users\test\Desktop\My Portfolio\work-1.png" alt="">
                    <div class="layer">
                        <h2>Social Media App</h2>
                        <p>In the realm of social media app development, I have successfully created engaging platforms that foster meaningful connections and interactions. Through intuitive user interfaces, real-time updates, and robust privacy controls, I empower users to share their stories and connect with others in a safe and enjoyable environment.</p>
                        <a href="#"><i class="fas fa-external-link-alt"></i></a>
                    </div>
                </div>
                <div class="work">
                    <img src="C:\Users\test\Desktop\My Portfolio\work-2.png" alt="">
                    <div class="layer">
                        <h2>Music App</h2>
                        <p>In the realm of music app development, I have crafted platforms that elevate the way users discover, listen, and share their favorite tunes. My music apps boast sleek and intuitive interfaces that enable effortless navigation and access to an extensive library of songs. </p>
                        <a href="#"><i class="fas fa-external-link-alt"></i></a>
                    </div>
                </div>
                <div class="work">
                    <img src="C:\Users\test\Desktop\My Portfolio\work-3.png" alt="">
                    <div class="layer">
                        <h2>Online Shopping App</h2>
                        <p>As an app developer with a focus on e-commerce, I have designed and developed online shopping applications that offer a seamless and secure buying experience. With a user-centric approach, I optimize the app's interface to simplify product discovery, checkout processes, and payment methods.</p>
                        <a href="#"><i class="fas fa-external-link-alt"></i></a>
                    </div>
                </div>
            </div>
            <a href="" class="btn">See more</a>
        </div>
    </div>

    <!-- ----------CONTACT---------- -->
    <div id="contact">
        <div class="container">
            <div class="row">
                <div class="contact-left">
                    <h1 class="sub-title">Contact Me</h1>
                    <p><i class="fas fa-paper-plane"></i> <a href="mailto:rehaanashraf2005@gmail.com"style="text-decoration: none; color: white";>rehaanashraf2005@gmail.com</a></p>

                    <p><i class="fas fa-phone-square-alt"></i> <a href="tel:+918008556781"style="text-decoration: none; color: white">8008556781</a></p>

                    <div class="social-icons">
                        <a href="https://www.facebook.com/mahammad.sameera"><i class="fab fa-facebook"></i></a>
                        <a href="https://twitter.com/REHAANASHRAF3?t=H2AcsOEBsr14IO2KbRJtlA&s=08"><i class="fab fa-twitter-square"></i></a>
                        <a href="https://instagram.com/madboy__rehaan?utm_source=qr&igshid=NGExMmI2YTkyZg%3D%3D"><i class="fab fa-instagram"></i></a>
                        <a href="https://in.linkedin.com/in/rehaan-ashraf-90a8b2278"><i class="fab fa-linkedin"></i></a>
                    </div>
                    <a href="C:\Users\test\Desktop\My Portfolio\MY CV.docx" download class="btn btn2">Download CV</a>
                </div>
                <div class="contact-right">
                    <form>
                        <input type="text" name="Name" placeholder="Your Name" required>
                        <input type="email" name="Email" placeholder="Your Email" required>
                        <textarea name="Message" rows="6" placeholder="Your Message"></textarea>
                        <button type="submit" class="btn btn3">submit</button>
                    </form>
                </div>
            </div>
        </div>
        <div class="copyright">
            <p>copyright @ Rehaan. Made with <i class="fas fa-heart"></i> by Rehaan</p>
        </div>
    </div>



    <script>
        var tabLinks = document.getElementsByClassName('tab-links');
        var tabContents = document.getElementsByClassName('tab-contents');

        function openTab(tabName) {
            for (tabLink of tabLinks) {
                tabLink.classList.remove('active-link');
            }
            for (tabContent of tabContents) {
                tabContent.classList.remove('active-tab');
            }
            event.currentTarget.classList.add('active-link');
            document.getElementById(tabName).classList.add('active-tab');
        }

        // JavaScript for handling the mobile navigation menu
        document.querySelector('.fas.fa-bars').addEventListener('click', function () {
            document.querySelector('nav ul').classList.toggle('show');
        });

        document.querySelector('.fas.fa-times').addEventListener('click', function () {
            document.querySelector('nav ul').classList.remove('show');
        });

    </script>
</body>

</html>

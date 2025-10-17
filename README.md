<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Minimalist Portfolio</title>
    <style>
       
        :root {
            --primary-color: #333; 
            --accent-color: #00bcd4; 
            --background-light: #f9f9f9;
            --background-dark: #ffffff;
            --font-family: 'Helvetica Neue', Arial, sans-serif;
        }
ase Styles */
        body {
            font-family: var(--font-family);
            margin: 0;
            padding: 0;
            background-color: var(--background-light);
            color: var(--primary-color);
            line-height: 1.6;
            text-align: center;
        }

       
        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 0 20px;
        }

        header {
            background-color: var(--background-dark);
            border-bottom: 1px solid #eee;
            padding: 1.5rem 0;
            box-shadow: 0 1px 3px rgba(0, 0, 0, 0.05);
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        header h1 {
            margin: 0;
            font-size: 1.8rem;
            color: var(--accent-color);
            font-weight: 700;
        }

        nav a {
            color: var(--primary-color);
            text-decoration: none;
            margin-left: 20px;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--accent-color);
        }

        section {
            padding: 80px 0;
            text-align: center;
        }

        section:nth-child(even) {
            background-color: var(--background-dark);
        }

        h2 {
            color: var(--primary-color);
            font-size: 2.2rem;
            margin-bottom: 40px;
            text-transform: uppercase;
            letter-spacing: 2px;
            font-weight: 300;
            position: relative;
            padding-bottom: 10px;
        }

        h2::after {
            content: '';
            width: 50px;
            height: 3px;
            background-color: var(--accent-color);
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
        }

        #about p {
            font-size: 1.15rem;
            max-width: 800px;
            margin: 0 auto 20px;
        }

    
        .timeline {
            max-width: 800px;
            margin: 0 auto;
        }

        .timeline-item {
            text-align: left;
            padding: 20px 0;
            border-bottom: 1px solid #ddd;
        }

        .timeline-item:last-child {
            border-bottom: none;
        }

        .timeline-item span.dates {
            display: block;
            font-size: 0.9rem;
            color: var(--accent-color);
            margin-bottom: 5px;
        }

        .timeline-item h3 {
            margin: 0;
            font-size: 1.25rem;
            font-weight: 600;
        }

        .timeline-item p {
            margin: 5px 0 0 0;
            color: #666;
            font-size: 1rem;
        }

       
        .skills-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
            margin-top: 30px;
            max-width: 900px;
            margin-left: auto;
            margin-right: auto;
        }

        .skill-tag {
            background-color: #fff;
            color: var(--primary-color);
            padding: 8px 15px;
            border-radius: 4px;
            border: 1px solid #ddd;
            font-weight: 500;
            font-size: 0.9rem;
            transition: background-color 0.3s, border-color 0.3s;
        }
        
        .skill-tag:hover {
            background-color: var(--accent-color);
            color: white;
            border-color: var(--accent-color);
        }

        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 30px;
            text-align: left;
            margin-top: 30px;
        }

        .project-card {
            background-color: var(--background-dark);
            border-radius: 8px;
            padding: 25px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.08);
            transition: box-shadow 0.3s;
        }

        .project-card:hover {
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.1);
        }

        .project-card h3 {
            color: var(--accent-color);
            margin-top: 0;
            font-size: 1.5rem;
        }

        .project-card a {
            display: inline-block;
            margin-top: 15px;
            color: var(--accent-color);
            text-decoration: none;
            font-weight: bold;
            border-bottom: 2px solid transparent;
        }

        .project-card a:hover {
             border-bottom: 2px solid var(--accent-color);
        }

        .contact-links {
            margin-top: 20px;
        }

        .contact-links a {
            display: inline-block;
            padding: 10px 25px;
            background-color: var(--accent-color);
            color: white;
            text-decoration: none;
            border-radius: 5px;
            margin: 0 10px;
            font-weight: 600;
            transition: background-color 0.3s;
        }

        .contact-links a:hover {
            background-color: #0097a7; /* Slightly darker teal */
        }

        footer {
            padding: 20px 0;
            background-color: var(--primary-color);
            color: white;
            font-size: 0.9rem;
        }

        @media (max-width: 600px) {
            .header-content {
                flex-direction: column;
            }
            nav {
                margin-top: 15px;
            }
            nav a {
                margin: 0 10px;
            }
            section {
                padding: 50px 0;
            }
        }

    </style>
</head>
<body>

    <header>
        <div class="container header-content">
            <h1>A BINDU</h1>
            <nav>
                <a href="#about">About</a>
                <a href="#education">Education</a>
                <a href="#skills">Skills</a>
                <a href="#projects">Projects</a>
                <a href="#contact">Contact</a>
            </nav>
        </div>
    </header>

    <section id="about">
        <div class="container">
            <h2>About Me</h2>
            <p>Hello! I am A Bindu dedicated to building elegant and efficient web applications, I thrive on solving complex problems and delivering high-quality, scalable code.</p>
            <p>I believe in clean design, continuous improvement, and always putting the user experience first.</p>
        </div>
    </section>

    <section id="education">
        <div class="container timeline">
            <h2>Education</h2>
            
            <div class="timeline-item">
                <span class="dates">2024| 7.78 CGPA</span>
                <h3>Bachelor of Technology (B.Tech) in Artificial Intelligence & Data Science</h3>
                <p> Mother Theresa Institute of Engineering and Technology</p>
            </div>

            <div class="timeline-item">
                <span class="dates">2022 - 2024 | 86.5%</span>
                <h3>Intermediate / MPC</h3>
                <p> Mother Theresa Junior College, Mumbai</p>
            </div>

            <div class="timeline-item">
                <span class="dates">2022 | 70%</span>
                <h3>Secondary School (10th Standard)</h3>
                <p>AP Model School</p>
            </div>

        </div>
    </section>

    <section id="skills">
        <div class="container">
            <h2>Technical Skills</h2>
            <div class="skills-container">
                <div class="skill-tag">C</div>
              <div class="skill-tag">JAVA</div>
                <div class="skill-tag">Python</div>
          
                <div class="skill-tag">C/C++</div>
                <div class="skill-tag">HTML5 & CSS3</div>
                <div class="skill-tag">Communication Skills</div>
                   <div class="skill-tag">Leadership Skills</div>
            </div>
        </div>
    </section>


    <section id="projects">
        <div class="container">
            <h2>Featured Projects</h2>
            <div class="project-grid">
                <div class="project-card">
                    <h3>E-commerce Platform</h3>
                    <p>A scalable full-stack application with user authentication, inventory management, and a custom payment flow.</p>
                    
                </div>
              
                <div class="project-card">
                    <h3>Portfolio Website V3</h3>
                    <p>Designed and coded this very website from scratch, focusing on mobile responsiveness and modern CSS techniques (Flexbox and Grid).</p>
                    
                </div>
            </div>
        </div>
    </section>

    <section id="contact">
        <div class="container">
            <h2>Get In Touch</h2>
      
            <div class="contact-links">
               
                 <p><i class="fas fa-envelope"></i> <a href="mailto:bindureddy634@gmail.com">Email Me</a></p><br>
               
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; A Bindu .</p>
        </div>
    </footer>

</body>
</html>

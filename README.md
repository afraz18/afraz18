<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Afraj Charaniya - GitHub Profile</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
            color: #f0f6fc;
            line-height: 1.6;
            padding: 2rem;
            min-height: 100vh;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
            background: rgba(13, 17, 23, 0.85);
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.4);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        header {
            text-align: center;
            margin-bottom: 2.5rem;
            padding-bottom: 1.5rem;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            border: 4px solid #58a6ff;
            margin-bottom: 1.5rem;
            box-shadow: 0 0 20px rgba(88, 166, 255, 0.3);
        }
        
        h1 {
            font-size: 2.8rem;
            margin-bottom: 0.5rem;
            color: #58a6ff;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.5);
        }
        
        h2 {
            font-size: 1.8rem;
            margin: 1.8rem 0 1rem;
            color: #f0f6fc;
            padding-bottom: 0.5rem;
            border-bottom: 2px solid #58a6ff;
            display: inline-block;
        }
        
        h3 {
            font-size: 1.4rem;
            margin: 1.5rem 0 0.8rem;
            color: #c9d1d9;
        }
        
        p {
            margin-bottom: 1.2rem;
            font-size: 1.1rem;
        }
        
        .tagline {
            font-size: 1.4rem;
            color: #c9d1d9;
            margin-bottom: 1.5rem;
        }
        
        .contact-info {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 1.5rem;
            margin: 1.5rem 0;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }
        
        .btn {
            display: inline-block;
            background: linear-gradient(to right, #238636, #2ea043);
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 6px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            margin: 0.5rem;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
        }
        
        .btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
            background: linear-gradient(to right, #2ea043, #3fb950);
        }
        
        .btn-outline {
            background: transparent;
            border: 2px solid #58a6ff;
            color: #58a6ff;
        }
        
        .btn-outline:hover {
            background: rgba(88, 166, 255, 0.1);
        }
        
        .card {
            background: rgba(22, 27, 34, 0.6);
            border-radius: 10px;
            padding: 1.5rem;
            margin-bottom: 1.5rem;
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
            border-color: rgba(88, 166, 255, 0.3);
        }
        
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 1.5rem;
            margin: 1.5rem 0;
        }
        
        .skill-category {
            margin-bottom: 2rem;
        }
        
        .skills-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 0.8rem;
        }
        
        .skill-tag {
            background: rgba(88, 166, 255, 0.15);
            color: #79c0ff;
            padding: 0.5rem 1rem;
            border-radius: 20px;
            font-size: 0.9rem;
            border: 1px solid rgba(88, 166, 255, 0.3);
            transition: all 0.3s ease;
        }
        
        .skill-tag:hover {
            background: rgba(88, 166, 255, 0.3);
            transform: scale(1.05);
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin: 2rem 0;
        }
        
        .social-icon {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(135deg, #1f6feb, #58a6ff);
            color: white;
            font-size: 1.5rem;
            text-decoration: none;
            transition: all 0.3s ease;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
        }
        
        .social-icon:hover {
            transform: translateY(-5px) rotate(5deg);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.3);
        }
        
        .experience-item {
            margin-bottom: 1.5rem;
            padding-bottom: 1.5rem;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .experience-item:last-child {
            border-bottom: none;
        }
        
        .date {
            color: #8b949e;
            font-style: italic;
            margin-bottom: 0.5rem;
        }
        
        .icon-text {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            margin-bottom: 0.5rem;
        }
        
        .stats {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin: 2rem 0;
            text-align: center;
        }
        
        .stat-item {
            padding: 1rem;
        }
        
        .stat-number {
            font-size: 2.5rem;
            font-weight: 700;
            color: #58a6ff;
            display: block;
        }
        
        .stat-label {
            color: #8b949e;
            font-size: 1rem;
        }
        
        @media (max-width: 768px) {
            .grid {
                grid-template-columns: 1fr;
            }
            
            .contact-info {
                flex-direction: column;
                align-items: center;
            }
            
            h1 {
                font-size: 2.2rem;
            }
            
            .tagline {
                font-size: 1.2rem;
            }
        }
        
        .highlight {
            color: #58a6ff;
            font-weight: 600;
        }
        
        .quote {
            font-style: italic;
            border-left: 4px solid #58a6ff;
            padding-left: 1rem;
            margin: 1.5rem 0;
            color: #8b949e;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <img src="https://avatars.githubusercontent.com/u/99283319?v=4" alt="Afraj Charaniya" class="profile-img">
            <h1>Afraj Charaniya</h1>
            <p class="tagline">Full-Stack Developer & Data Scientist | MCA Student</p>
            
            <div class="contact-info">
                <div class="contact-item">
                    <i class="fas fa-envelope"></i>
                    <span>afrajcharniya264@gmail.com</span>
                </div>
                <div class="contact-item">
                    <i class="fas fa-phone"></i>
                    <span>8511290712</span>
                </div>
                <div class="contact-item">
                    <i class="fas fa-map-marker-alt"></i>
                    <span>Vadodara, Gujarat, India</span>
                </div>
            </div>
            
            <div>
                <a href="https://www.linkedin.com/in/afraj-charaniya-042484255" class="btn" target="_blank">
                    <i class="fab fa-linkedin"></i> LinkedIn
                </a>
                <a href="https://github.com/afrajcharaniya" class="btn btn-outline" target="_blank">
                    <i class="fab fa-github"></i> GitHub
                </a>
                <a href="#" class="btn" onclick="alert('Resume downloaded!')">
                    <i class="fas fa-download"></i> Download Resume
                </a>
            </div>
        </header>
        
        <section>
            <h2>About Me</h2>
            <div class="card">
                <p>Results-driven B.Sc. IT graduate from the University of Mumbai, currently pursuing MCA. Experienced through five industry internships with firms like TCS, Deloitte, and IBM. Skilled in full-stack development, data science, cloud computing, and UI/UX.</p>
                
                <p class="quote">"Fast learner and collaborative team player with strong communication skills"</p>
                
                <div class="stats">
                    <div class="stat-item">
                        <span class="stat-number">5+</span>
                        <span class="stat-label">Internships</span>
                    </div>
                    <div class="stat-item">
                        <span class="stat-number">10+</span>
                        <span class="stat-label">Projects</span>
                    </div>
                    <div class="stat-item">
                        <span class="stat-number">15+</span>
                        <span class="stat-label">Skills</span>
                    </div>
                </div>
            </div>
        </section>
        
        <section>
            <h2>Experience</h2>
            <div class="grid">
                <div class="card">
                    <h3>Web Design & Development Intern</h3>
                    <p class="date">Internship Studio | Jun 2025 – Aug 2025</p>
                    <p>Spearheaded the development of responsive web pages using HTML, CSS, and PHP, improving project turnaround time by 30%.</p>
                </div>
                
                <div class="card">
                    <h3>Data Visualization Intern</h3>
                    <p class="date">Tata Consultancy Services | Jun 2025</p>
                    <p>Implemented interactive dashboards using Tableau and Power BI, enhancing data-driven decision-making for sample business cases.</p>
                </div>
                
                <div class="card">
                    <h3>Technology Intern</h3>
                    <p class="date">Deloitte | Jun 2025</p>
                    <p>Supported digital solution rollouts, contributing to cloud migration and application testing initiatives.</p>
                </div>
                
                <div class="card">
                    <h3>AI Intern</h3>
                    <p class="date">IBM | Feb 2025 - Jun 2025</p>
                    <p>Implemented basic AI workflows and machine learning algorithms, applying them in real-world-inspired case studies.</p>
                </div>
            </div>
        </section>
        
        <section>
            <h2>Technical Skills</h2>
            <div class="card">
                <div class="skill-category">
                    <h3>Programming Languages</h3>
                    <div class="skills-grid">
                        <span class="skill-tag">C</span>
                        <span class="skill-tag">C++</span>
                        <span class="skill-tag">Java</span>
                        <span class="skill-tag">Python</span>
                        <span class="skill-tag">JavaScript</span>
                        <span class="skill-tag">PHP</span>
                        <span class="skill-tag">SQL</span>
                        <span class="skill-tag">Shell Scripting</span>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h3>Web Development</h3>
                    <div class="skills-grid">
                        <span class="skill-tag">HTML5</span>
                        <span class="skill-tag">CSS3</span>
                        <span class="skill-tag">Bootstrap</span>
                        <span class="skill-tag">React.js</span>
                        <span class="skill-tag">Node.js</span>
                        <span class="skill-tag">jQuery</span>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h3>Data Science & Analytics</h3>
                    <div class="skills-grid">
                        <span class="skill-tag">Pandas</span>
                        <span class="skill-tag">NumPy</span>
                        <span class="skill-tag">Scikit-learn</span>
                        <span class="skill-tag">Matplotlib</span>
                        <span class="skill-tag">Power BI</span>
                        <span class="skill-tag">Tableau</span>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h3>Cloud & DevOps</h3>
                    <div class="skills-grid">
                        <span class="skill-tag">AWS</span>
                        <span class="skill-tag">Firebase</span>
                        <span class="skill-tag">Docker</span>
                        <span class="skill-tag">CI/CD</span>
                        <span class="skill-tag">Git</span>
                        <span class="skill-tag">GitHub</span>
                    </div>
                </div>
            </div>
        </section>
        
        <section>
            <h2>Projects</h2>
            <div class="card">
                <h3>Furniture E-Commerce Website Management</h3>
                <p class="date">December 2024 – April 2025</p>
                <p>Developed a complete e-commerce website for online furniture sales with product catalog, cart, and checkout system.</p>
                <p><span class="highlight">Technologies used:</span> HTML, CSS, JavaScript, PHP, MySQL, Bootstrap</p>
                <a href="#" class="btn btn-outline">
                    <i class="fas fa-external-link-alt"></i> View Project
                </a>
            </div>
        </section>
        
        <section>
            <h2>Certifications</h2>
            <div class="grid">
                <div class="card">
                    <h3>Data Visualization</h3>
                    <p>Tata Consultancy Services</p>
                    <p>Gained hands-on experience in creating dashboards and visual insights from data.</p>
                </div>
                
                <div class="card">
                    <h3>Technology Consulting</h3>
                    <p>Deloitte Company</p>
                    <p>Participated in a virtual consulting program applying IT solutions to real-world cases.</p>
                </div>
                
                <div class="card">
                    <h3>Python Data Science</h3>
                    <p>IBM Internship</p>
                    <p>Applied data science techniques for real business use cases using Python.</p>
                </div>
                
                <div class="card">
                    <h3>AWS Solutions Architect</h3>
                    <p>AWS Virtual Internship</p>
                    <p>Learned to design scalable, secure cloud architectures through real-world scenarios.</p>
                </div>
            </div>
        </section>
        
        <section>
            <h2>Get In Touch</h2>
            <div class="card">
                <p>I'm always open to discussing new projects, creative ideas, or opportunities to be part of your vision.</p>
                
                <div class="social-links">
                    <a href="https://www.linkedin.com/in/afraj-charaniya-042484255" class="social-icon" target="_blank">
                        <i class="fab fa-linkedin-in"></i>
                    </a>
                    <a href="https://github.com/afrajcharaniya" class="social-icon" target="_blank">
                        <i class="fab fa-github"></i>
                    </a>
                    <a href="mailto:afrajcharniya264@gmail.com" class="social-icon">
                        <i class="far fa-envelope"></i>
                    </a>
                    <a href="https://twitter.com" class="social-icon" target="_blank">
                        <i class="fab fa-twitter"></i>
                    </a>
                </div>
                
                <div style="text-align: center;">
                    <a href="#" class="btn">
                        <i class="fas fa-paper-plane"></i> Send Message
                    </a>
                </div>
            </div>
        </section>
    </div>

    <script>
        // Simple animation for skills on hover
        document.querySelectorAll('.skill-tag').forEach(tag => {
            tag.addEventListener('mouseover', function() {
                this.style.transform = 'scale(1.1)';
                this.style.transition = 'transform 0.2s ease';
            });
            
            tag.addEventListener('mouseout', function() {
                this.style.transform = 'scale(1)';
            });
        });
        
        // Animate stats counting up
        function animateValue(element, start, end, duration) {
            let startTimestamp = null;
            const step = (timestamp) => {
                if (!startTimestamp) startTimestamp = timestamp;
                const progress = Math.min((timestamp - startTimestamp) / duration, 1);
                element.innerHTML = Math.floor(progress * (end - start) + start);
                if (progress < 1) {
                    window.requestAnimationFrame(step);
                }
            };
            window.requestAnimationFrame(step);
        }
        
        // Start animations when page loads
        window.addEventListener('load', function() {
            const statElements = document.querySelectorAll('.stat-number');
            animateValue(statElements[0], 0, 5, 2000);
            animateValue(statElements[1], 0, 10, 2000);
            animateValue(statElements[2], 0, 15, 2000);
        });
    </script>
</body>
</html>

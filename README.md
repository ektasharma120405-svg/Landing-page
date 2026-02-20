!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Internship Task 2 - Level 3</title>
    <style>
        :root {
            --pastel-blue: #A7C7E7;
            --pastel-green: #C1E1C1;
            --pastel-peach: #FFDAB9;
            --pastel-lavender: #E6E6FA;
            --pastel-pink: #FFB6C1;
            --dark-text: #333333;
            --light-text: #555555;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f9f9f9;
            color: var(--dark-text);
            line-height: 1.6;
        }

        header {
            background: linear-gradient(135deg, var(--pastel-blue), var(--pastel-lavender));
            padding: 2rem 0;
            text-align: center;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
        }

        .logo {
            font-size: 2rem;
            font-weight: 700;
            color: white;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
            margin-bottom: 1rem;
        }

        h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: white;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }

        .intro {
            background-color: white;
            padding: 3rem 2rem;
            border-radius: 10px;
            margin: 2rem auto;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.05);
            text-align: center;
        }

        .intro p {
            color: var(--light-text);
            font-size: 1.1rem;
            max-width: 800px;
            margin: 0 auto;
        }

        .highlights {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 2rem;
            margin: 3rem 0;
        }

        .highlight-card {
            background-color: white;
            border-radius: 10px;
            padding: 2rem;
            width: 300px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            text-align: center;
        }

        .highlight-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
        }

        .highlight-card:nth-child(1) {
            border-top: 5px solid var(--pastel-blue);
        }

        .highlight-card:nth-child(2) {
            border-top: 5px solid var(--pastel-green);
        }

        .highlight-card:nth-child(3) {
            border-top: 5px solid var(--pastel-pink);
        }

        .highlight-icon {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: var(--light-text);
        }

        .qualifications {
            background-color: var(--pastel-peach);
            padding: 3rem 2rem;
            border-radius: 10px;
            margin: 2rem auto;
        }

        .qualifications h2 {
            text-align: center;
            margin-bottom: 2rem;
            color: var(--dark-text);
        }

        .skills-list {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 1.5rem;
        }

        .skill {
            background-color: white;
            padding: 1rem 1.5rem;
            border-radius: 50px;
            font-weight: 500;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
        }

        .cta-section {
            text-align: center;
            margin: 4rem 0;
        }

        .cta-button {
            display: inline-block;
            background: linear-gradient(135deg, var(--pastel-blue), var(--pastel-lavender));
            color: white;
            padding: 1rem 2.5rem;
            font-size: 1.2rem;
            font-weight: 600;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            text-decoration: none;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
        }

        .cta-button.secondary {
            background: white;
            color: var(--pastel-blue);
            margin-left: 1rem;
            border: 2px solid var(--pastel-blue);
        }

        footer {
            background: linear-gradient(135deg, var(--pastel-blue), var(--pastel-lavender));
            color: white;
            padding: 3rem 0;
            text-align: center;
        }

        .contact-info {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 2rem;
            margin-top: 2rem;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .contact-icon {
            font-size: 1.2rem;
        }

        @media (max-width: 768px) {
            h1 {
                font-size: 2rem;
            }

            .highlight-card {
                width: 100%;
            }

            .cta-button {
                display: block;
                margin: 1rem auto;
                width: 80%;
            }

            .cta-button.secondary {
                margin-left: auto;
            }
        }

        /* Animation classes */
        .fade-in {
            animation: fadeIn 1s ease-in;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
            }

            to {
                opacity: 1;
            }
        }

        .slide-up {
            animation: slideUp 0.8s ease-out;
        }

        @keyframes slideUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }

            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>

<body>
    <header class="fade-in">
        <div class="container">
            <div class="logo">Cognifyz Technologies</div>
            <h1>Web Developer Internship Opportunities</h1>
        </div>
    </header>

    <main class="container">
        <section class="intro slide-up">
            <h2>Launch Your Web Development Career</h2>
            <p>Join our 3-6 month intensive internship program designed to give you hands-on experience with real-world
                projects. Work alongside experienced developers, learn industry best practices, and build a portfolio
                that stands out.</p>
        </section>

        <section class="highlights">
            <div class="highlight-card slide-up" style="animation-delay: 0.2s;">
                <div class="highlight-icon">
                    <i class="fas fa-laptop-code"></i>
                </div>
                <h3>Real-World Experience</h3>
                <p>Work on live projects that impact our business and clients. No dummy projects here!</p>
            </div>

            <div class="highlight-card slide-up" style="animation-delay: 0.4s;">
                <div class="highlight-icon">
                    <i class="fas fa-chalkboard-teacher"></i>
                </div>
                <h3>Expert Mentorship</h3>
                <p>Learn from senior developers with 5+ years of industry experience.</p>
            </div>

            <div class="highlight-card slide-up" style="animation-delay: 0.6s;">
                <div class="highlight-icon">
                    <i class="fas fa-network-wired"></i>
                </div>
                <h3>Career Opportunities</h3>
                <p>Top performers may receive full-time job offers upon completion.</p>
            </div>
        </section>

        <section class="qualifications slide-up" style="animation-delay: 0.8s;">
            <h2>Desired Skills & Technologies</h2>
            <div class="skills-list">
                <div class="skill">HTML5</div>
                <div class="skill">CSS3</div>
                <div class="skill">JavaScript</div>
                <div class="skill">React</div>
                <div class="skill">Node.js</div>
                <div class="skill">Git</div>
                <div class="skill">Responsive Design</div>
                <div class="skill">Problem Solving</div>
            </div>
        </section>

        <section class="cta-section slide-up" style="animation-delay: 1s;">
            <h2>Ready to Start Your Journey?</h2>
            <p>Applications are open for our next cohort beginning next month.</p>
            <div style="margin-top: 2rem;">
                <a href="#apply" class="cta-button" id="applyButton">Apply Now</a>
                <a href="#learn-more" class="cta-button secondary">Learn More</a>
            </div>
        </section>
    </main>

    <footer class="fade-in" style="animation-delay: 1.2s;">
        <div class="container">
            <h3>Contact Us</h3>
            <p>Have questions about the internship program? Get in touch!</p>

            <div class="contact-info">
                <div class="contact-item">
                    <span class="contact-icon"><i class="fas fa-envelope"></i></span>
                    <span>internships@cognifyz.com</span>
                </div>
                <div class="contact-item">
                    <span class="contact-icon"><i class="fas fa-phone"></i></span>
                    <span>+1 (555) 123-4567</span>
                </div>
                <div class="contact-item">
                    <span class="contact-icon"><i class="fas fa-map-marker-alt"></i></span>
                    <span>123 Tech Park, Silicon Valley, CA</span>
                </div>
            </div>

            <div style="margin-top: 2rem;">
                <a href="#" style="color: white; margin: 0 0.5rem;"><i class="fab fa-linkedin fa-lg"></i></a>
                <a href="#" style="color: white; margin: 0 0.5rem;"><i class="fab fa-twitter fa-lg"></i></a>
                <a href="#" style="color: white; margin: 0 0.5rem;"><i class="fab fa-github fa-lg"></i></a>
            </div>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function () {
            // Smooth scroll for anchor links
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    e.preventDefault();

                    if (this.getAttribute('href') === '#apply') {
                        // Show application form (could be expanded in a real implementation)
                        alert('Application form would open here!');
                        return;
                    }

                    if (this.getAttribute('href') === '#learn-more') {
                        // Show more details (could be expanded)
                        alert('More information about the program would be displayed here!');
                        return;
                    }

                    document.querySelector(this.getAttribute('href')).scrollIntoView({
                        behavior: 'smooth'
                    });
                });
            });

            // Animation on scroll (could be enhanced with Intersection Observer)
            const animateOnScroll = () => {
                const elements = document.querySelectorAll('.slide-up, .fade-in');

                elements.forEach(element => {
                    const elementPosition = element.getBoundingClientRect().top;
                    const windowHeight = window.innerHeight;

                    if (elementPosition < windowHeight - 100) {
                        element.style.opacity = '1';
                        element.style.transform = 'translateY(0)';
                    }
                });
            };

            window.addEventListener('scroll', animateOnScroll);
            animateOnScroll(); // Run once on load
        });
    </script>
</body>

</html>

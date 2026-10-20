<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional Resume</title>
    <style>
        :root {
            --primary-color: #2c3e50;
            --accent-color: #3498db;
            --text-color: #333333;
            --light-bg: #f8f9fa;
            --border-color: #e2e8f0;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            color: var(--text-color);
            line-height: 1.6;
            background-color: #fff;
            padding: 40px 20px;
        }

        .resume-container {
            max-width: 800px;
            margin: 0 auto;
            background: #fff;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
            border: 1px solid var(--border-color);
            display: grid;
            grid-template-columns: 1fr 2fr;
        }

        /* Sidebar Styles */
        .sidebar {
            background-color: var(--light-bg);
            padding: 40px 30px;
            border-right: 1px solid var(--border-color);
        }

        .profile-section {
            margin-bottom: 30px;
        }

        .name {
            font-size: 24px;
            font-weight: 700;
            color: var(--primary-color);
            line-height: 1.2;
            margin-bottom: 5px;
        }

        .title {
            font-size: 14px;
            font-weight: 600;
            color: var(--accent-color);
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .contact-section, .skills-section, .education-section {
            margin-bottom: 30px;
        }

        h3 {
            font-size: 14px;
            text-transform: uppercase;
            letter-spacing: 1px;
            color: var(--primary-color);
            border-bottom: 2px solid var(--accent-color);
            padding-bottom: 5px;
            margin-bottom: 15px;
        }

        .contact-item {
            font-size: 13px;
            margin-bottom: 10px;
            word-break: break-all;
        }

        .contact-item a {
            color: var(--text-color);
            text-decoration: none;
        }

        .contact-item a:hover {
            color: var(--accent-color);
        }

        .skills-list {
            list-style: none;
        }

        .skills-list li {
            font-size: 13px;
            margin-bottom: 8px;
            background: #fff;
            padding: 6px 10px;
            border-radius: 4px;
            border: 1px solid var(--border-color);
        }

        /* Main Content Styles */
        .main-content {
            padding: 40px 30px;
        }

        .section {
            margin-bottom: 30px;
        }

        .summary-text {
            font-size: 14px;
            color: #555;
        }

        .job {
            margin-bottom: 20px;
        }

        .job-header {
            display: flex;
            justify-content: space-between;
            align-items: baseline;
            margin-bottom: 5px;
        }

        .job-title {
            font-size: 15px;
            font-weight: 700;
            color: var(--primary-color);
        }

        .job-company {
            font-size: 14px;
            font-weight: 600;
            color: var(--accent-color);
            margin-bottom: 5px;
        }

        .job-date {
            font-size: 12px;
            color: #777;
            font-weight: 500;
        }

        .job-description {
            font-size: 13px;
            padding-left: 15px;
        }

        .job-description li {
            margin-bottom: 5px;
        }

        .edu-item {
            margin-bottom: 15px;
        }

        .edu-degree {
            font-size: 14px;
            font-weight: 700;
            color: var(--primary-color);
        }

        .edu-school {
            font-size: 13px;
            color: #555;
        }

        .edu-date {
            font-size: 12px;
            color: #777;
        }

        /* Print styles */
        @media print {
            body {
                background: #fff;
                padding: 0;
            }
            .resume-container {
                border: none;
                box-shadow: none;
                max-width: 100%;
            }
        }

        /* Responsive design for smaller screens */
        @media (max-width: 768px) {
            .resume-container {
                grid-template-columns: 1fr;
            }
            .sidebar {
                border-right: none;
                border-bottom: 1px solid var(--border-color);
            }
        }
    </style>
</head>
<body>

    <div class="resume-container">
        <!-- Sidebar -->
        <aside class="sidebar">
            <div class="profile-section">
                <h1 class="name">Jane Doe</h1>
                <div class="title">Software Engineer</div>
            </div>

            <div class="contact-section">
                <h3>Contact</h3>
                <div class="contact-item">📍 San Francisco, CA</div>
                <div class="contact-item">📞 (555) 123-4567</div>
                <div class="contact-item">✉️ <a href="mailto:jane.doe@example.com">jane.doe@example.com</a></div>
                <div class="contact-item">🌐 <a href="https://linkedin.com" target="_blank">linkedin.com/in/janedoe</a></div>
                <div class="contact-item">💻 <a href="https://github.com" target="_blank">github.com/janedoe</a></div>
            </div>

            <div class="skills-section">
                <h3>Skills</h3>
                <ul class="skills-list">
                    <li>JavaScript / TypeScript</li>
                    <li>React & Node.js</li>
                    <li>HTML5 / CSS3 / Tailwind</li>
                    <li>RESTful APIs & GraphQL</li>
                    <li>Git & CI/CD Pipelines</li>
                    <li>Agile / Scrum Methodologies</li>
                </ul>
            </div>

            <div class="education-section">
                <h3>Education</h3>
                <div class="edu-item">
                    <div class="edu-degree">B.S. in Computer Science</div>
                    <div class="edu-school">University of California, Berkeley</div>
                    <div class="edu-date">Graduated: May 2022</div>
                </div>
            </div>
        </aside>

        <!-- Main Content -->
        <main class="main-content">
            <section class="section">
                <h3>Professional Summary</h3>
                <p class="summary-text">
                    Innovative and detail-oriented Software Engineer with over 4 years of experience designing, developing, and maintaining scalable web applications. Strong background in modern JavaScript frameworks and collaborative agile environments, dedicated to writing clean code and optimizing user experiences.
                </p>
            </section>

            <section class="section">
                <h3>Work Experience</h3>
                
                <div class="job">
                    <div class="job-header">
                        <span class="job-title">Full Stack Developer</span>
                        <span class="job-date">2023 – Present</span>
                    </div>
                    <div class="job-company">Tech Innovators Inc. — San Francisco, CA</div>
                    <ul class="job-description">
                        <li>Developed and maintained core features for a high-traffic SaaS platform using React, Node.js, and PostgreSQL.</li>
                        <li>Optimized application load times by 35% through code splitting, efficient state management, and asset optimization.</li>
                        <li>Collaborated closely with UX/UI designers and product managers to translate wireframes into responsive, accessible web components.</li>
                    </ul>
                </div>

                <div class="job">
                    <div class="job-header">
                        <span class="job-title">Junior Web Developer</span>
                        <span class="job-date">2022 – 2023</span>
                    </div>
                    <div class="job-company">Digital Solutions LLC — Oakland, CA</div>
                    <ul class="job-description">
                        <li>Built and deployed over 10 custom client-facing websites using HTML5, CSS3, and JavaScript.</li>
                        <li>Integrated RESTful APIs and third-party payment gateways (Stripe, PayPal) into e-commerce applications.</li>
                        <li>Participated in daily stand-ups and code reviews to maintain high coding standards and team alignment.</li>
                    </ul>
                </div>
            </section>

            <section class="section">
                <h3>Projects</h3>
                <div class="job">
                    <div class="job-header">
                        <span class="job-title">TaskFlow Project Management App</span>
                        <span class="job-date">2023</span>
                    </div>
                    <div class="job-company">Open Source / Personal Project</div>
                    <ul class="job-description">
                        <li>Engineered a full-stack Kanban board application featuring real-time task updates and drag-and-drop functionality.</li>
                        <li>Utilized React, Context API, Node.js, and Socket.io to support collaborative multi-user sessions.</li>
                    </ul>
                </div>
            </section>
        </main>
    </div>

</body>
</html>

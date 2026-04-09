<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trungdoublelift - Developer Portfolio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
 
        :root {
            --primary-color: #0ea5e9;
            --secondary-color: #1e293b;
            --accent-color: #f59e0b;
            --bg-color: #ffffff;
            --text-primary: #1e293b;
            --text-secondary: #64748b;
            --border-color: #e2e8f0;
            --code-bg: #f8fafc;
        }
 
        @media (prefers-color-scheme: dark) {
            :root {
                --bg-color: #0f172a;
                --text-primary: #f1f5f9;
                --text-secondary: #cbd5e1;
                --border-color: #334155;
                --code-bg: #1e293b;
            }
        }
 
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            background: linear-gradient(135deg, var(--bg-color) 0%, var(--bg-color) 100%);
            color: var(--text-primary);
            line-height: 1.6;
            min-height: 100vh;
        }
 
        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 60px 20px;
        }
 
        header {
            margin-bottom: 60px;
            text-align: center;
            animation: fadeInDown 0.6s ease;
        }
 
        .greeting {
            font-size: 18px;
            color: var(--primary-color);
            margin-bottom: 15px;
            font-weight: 600;
            letter-spacing: 2px;
            text-transform: uppercase;
        }
 
        h1 {
            font-size: 3.5rem;
            font-weight: 800;
            margin-bottom: 20px;
            background: linear-gradient(135deg, var(--primary-color) 0%, var(--accent-color) 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
 
        .quote {
            background: linear-gradient(135deg, rgba(14, 165, 233, 0.1) 0%, rgba(245, 158, 11, 0.1) 100%);
            border-left: 4px solid var(--primary-color);
            padding: 20px;
            border-radius: 8px;
            margin: 20px 0;
            font-style: italic;
            color: var(--text-primary);
            font-size: 1.1rem;
        }
 
        .quote .author {
            display: block;
            margin-top: 10px;
            color: var(--text-secondary);
            font-size: 0.95rem;
            font-style: normal;
        }
 
        .intro {
            font-size: 1.1rem;
            color: var(--text-primary);
            margin-top: 25px;
            line-height: 1.8;
        }
 
        hr {
            border: none;
            height: 2px;
            background: linear-gradient(90deg, transparent, var(--border-color), transparent);
            margin: 50px 0;
        }
 
        section {
            margin-bottom: 50px;
            animation: fadeInUp 0.6s ease;
        }
 
        section h2 {
            font-size: 2rem;
            margin-bottom: 25px;
            color: var(--text-primary);
            display: flex;
            align-items: center;
            gap: 12px;
        }
 
        section h3 {
            font-size: 1.3rem;
            margin: 25px 0 15px 0;
            color: var(--text-primary);
        }
 
        section p {
            color: var(--text-secondary);
            margin-bottom: 15px;
            line-height: 1.8;
            font-size: 1.05rem;
        }
 
        .tech-bar {
            margin: 25px 0;
            background: var(--code-bg);
            padding: 20px;
            border-radius: 8px;
            border: 1px solid var(--border-color);
            font-family: 'Monaco', 'Courier New', monospace;
            font-size: 0.95rem;
            overflow-x: auto;
        }
 
        .tech-bar div {
            margin: 10px 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
 
        .bar-container {
            flex: 1;
            height: 8px;
            background: var(--border-color);
            border-radius: 4px;
            margin: 0 15px;
            overflow: hidden;
        }
 
        .bar-fill {
            height: 100%;
            background: linear-gradient(90deg, var(--primary-color), var(--accent-color));
            border-radius: 4px;
        }
 
        ul, ol {
            margin-left: 25px;
            color: var(--text-secondary);
        }
 
        li {
            margin-bottom: 12px;
            line-height: 1.8;
        }
 
        li strong {
            color: var(--text-primary);
        }
 
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 25px 0;
            background: var(--code-bg);
            border-radius: 8px;
            overflow: hidden;
            border: 1px solid var(--border-color);
        }
 
        th, td {
            padding: 15px 20px;
            text-align: left;
            border-bottom: 1px solid var(--border-color);
        }
 
        th {
            background: linear-gradient(135deg, rgba(14, 165, 233, 0.1), rgba(245, 158, 11, 0.1));
            font-weight: 600;
            color: var(--text-primary);
        }
 
        tr:last-child td {
            border-bottom: none;
        }
 
        td strong {
            color: var(--text-primary);
        }
 
        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin: 25px 0;
        }
 
        .feature-card {
            background: var(--code-bg);
            border: 1px solid var(--border-color);
            padding: 20px;
            border-radius: 8px;
            transition: all 0.3s ease;
        }
 
        .feature-card:hover {
            transform: translateY(-5px);
            border-color: var(--primary-color);
            box-shadow: 0 10px 30px rgba(14, 165, 233, 0.1);
        }
 
        .feature-card strong {
            color: var(--primary-color);
            display: block;
            margin-bottom: 10px;
            font-size: 1.1rem;
        }
 
        .feature-card p {
            font-size: 0.95rem;
        }
 
        .icon {
            font-size: 24px;
            margin-right: 8px;
        }
 
        .links-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            margin: 25px 0;
        }
 
        .link-card {
            background: linear-gradient(135deg, rgba(14, 165, 233, 0.1), rgba(245, 158, 11, 0.05));
            border: 1px solid var(--border-color);
            padding: 15px 20px;
            border-radius: 8px;
            text-decoration: none;
            color: var(--primary-color);
            transition: all 0.3s ease;
            font-weight: 500;
        }
 
        .link-card:hover {
            background: linear-gradient(135deg, rgba(14, 165, 233, 0.2), rgba(245, 158, 11, 0.1));
            border-color: var(--primary-color);
            transform: translateX(5px);
        }
 
        .cta-button {
            display: inline-block;
            background: linear-gradient(135deg, var(--primary-color), var(--accent-color));
            color: white;
            padding: 15px 40px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            margin: 20px 0;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            font-size: 1rem;
        }
 
        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 35px rgba(14, 165, 233, 0.3);
        }
 
        footer {
            text-align: center;
            padding: 40px 20px;
            border-top: 1px solid var(--border-color);
            margin-top: 60px;
            color: var(--text-secondary);
        }
 
        footer p {
            margin: 10px 0;
        }
 
        .highlight {
            color: var(--primary-color);
            font-weight: 600;
        }
 
        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
 
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
 
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }
 
            section h2 {
                font-size: 1.6rem;
            }
 
            .container {
                padding: 40px 20px;
            }
 
            .features {
                grid-template-columns: 1fr;
            }
 
            .tech-bar div {
                flex-direction: column;
                align-items: flex-start;
            }
 
            .bar-container {
                margin: 10px 0;
                width: 100%;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header -->
        <header>
            <div class="greeting">👋 Welcome</div>
            <h1>I'm Trungdoublelift</h1>
            <div class="quote">
                <span>"The only way to do great work is to love what you do."</span>
                <span class="author">– Steve Jobs</span>
            </div>
            <p class="intro">
                Welcome to my corner of the internet. I'm a passionate developer on a mission to shape the future 
                of web development and create meaningful digital experiences.
            </p>
        </header>
 
        <hr>
 
        <!-- What I'm About -->
        <section>
            <h2><span class="icon">🌱</span>What I'm About</h2>
            <p>
                I'm currently deep in the world of <strong>Java</strong> and <strong>web development</strong>, constantly pushing boundaries and exploring innovative solutions. I believe the internet is the future of communication, and web development is the key to unlocking its potential.
            </p>
            <p>
                Every line of code I write is a step toward building something that matters—something that connects, inspires, and creates value for people around the world.
            </p>
        </section>
 
        <hr>
 
        <!-- My Vision -->
        <section>
            <h2><span class="icon">🚀</span>My Vision</h2>
            <p>
                The internet has revolutionized how we communicate. It's torn down geographical barriers, democratized information, and created endless possibilities for human connection. I'm committed to being at the forefront of this revolution.
            </p>
            
            <h3>Why I Do What I Do</h3>
            <ul>
                <li><strong>Innovation First</strong> — I believe in staying ahead of the curve, constantly learning and adapting to emerging technologies</li>
                <li><strong>Quality Over Quick</strong> — I write code that's clean, maintainable, and built to last</li>
                <li><strong>Impact Driven</strong> — Every project should solve a real problem and create genuine value</li>
                <li><strong>Continuous Growth</strong> — The moment I stop learning is the moment I stop growing</li>
            </ul>
        </section>
 
        <hr>
 
        <!-- Tech Focus -->
        <section>
            <h2><span class="icon">💻</span>Current Tech Focus</h2>
            <div class="tech-bar">
                <div>
                    <span>Java</span>
                    <div class="bar-container">
                        <div class="bar-fill" style="width: 85%;"></div>
                    </div>
                    <span>85%</span>
                </div>
                <div>
                    <span>Web Development</span>
                    <div class="bar-container">
                        <div class="bar-fill" style="width: 75%;"></div>
                    </div>
                    <span>75%</span>
                </div>
                <div>
                    <span>Frontend</span>
                    <div class="bar-container">
                        <div class="bar-fill" style="width: 65%;"></div>
                    </div>
                    <span>65%</span>
                </div>
                <div>
                    <span>Backend</span>
                    <div class="bar-container">
                        <div class="bar-fill" style="width: 70%;"></div>
                    </div>
                    <span>70%</span>
                </div>
            </div>
 
            <h3>Learning & Exploring</h3>
            <ul>
                <li>Advanced Java patterns and frameworks</li>
                <li>Modern web development practices</li>
                <li>Full-stack application development</li>
                <li>Performance optimization</li>
                <li>Cloud-native technologies</li>
            </ul>
        </section>
 
        <hr>
 
        <!-- Core Values -->
        <section>
            <h2><span class="icon">🎯</span>Core Values</h2>
            <table>
                <thead>
                    <tr>
                        <th>Value</th>
                        <th>Description</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td><strong>Excellence</strong></td>
                        <td>Striving for the best in every project</td>
                    </tr>
                    <tr>
                        <td><strong>Curiosity</strong></td>
                        <td>Never settling, always learning</td>
                    </tr>
                    <tr>
                        <td><strong>Collaboration</strong></td>
                        <td>Growing together with the community</td>
                    </tr>
                    <tr>
                        <td><strong>Integrity</strong></td>
                        <td>Building things the right way</td>
                    </tr>
                    <tr>
                        <td><strong>Impact</strong></td>
                        <td>Creating solutions that matter</td>
                    </tr>
                </tbody>
            </table>
        </section>
 
        <hr>
 
        <!-- Key Beliefs -->
        <section>
            <h2><span class="icon">🌟</span>Key Beliefs</h2>
            <ul>
                <li>The best developers are lifelong learners</li>
                <li>Simplicity is the ultimate sophistication</li>
                <li>Community thrives on shared knowledge</li>
                <li>Great code is readable code</li>
                <li>Technology should serve humanity</li>
            </ul>
        </section>
 
        <hr>
 
        <!-- My Journey -->
        <section>
            <h2><span class="icon">📈</span>My Journey</h2>
            <p>
                I'm on an exciting journey of growth and discovery. Every day brings new challenges to solve, new technologies to explore, and new opportunities to make a difference.
            </p>
            
            <h3>What Drives Me</h3>
            <ul>
                <li>Solving complex problems with elegant solutions</li>
                <li>Building scalable, maintainable applications</li>
                <li>Contributing to the open-source community</li>
                <li>Mentoring and learning from others</li>
                <li>Creating tools that improve people's lives</li>
            </ul>
        </section>
 
        <hr>
 
        <!-- What's Next -->
        <section>
            <h2><span class="icon">🔥</span>What's Next</h2>
            <p>I'm constantly evolving. Here's what's on my radar:</p>
            <div class="features">
                <div class="feature-card">
                    <strong>🎓 Mastering Java</strong>
                    <p>Deep diving into enterprise-level Java development</p>
                </div>
                <div class="feature-card">
                    <strong>🌐 Web Mastery</strong>
                    <p>Becoming an expert in full-stack web development</p>
                </div>
                <div class="feature-card">
                    <strong>💼 Open Source</strong>
                    <p>Contributing to meaningful projects</p>
                </div>
                <div class="feature-card">
                    <strong>🚀 Building</strong>
                    <p>Creating applications that make a real difference</p>
                </div>
                <div class="feature-card">
                    <strong>📚 Teaching</strong>
                    <p>Sharing knowledge with the next generation</p>
                </div>
            </div>
        </section>
 
        <hr>
 
        <!-- Philosophy -->
        <section>
            <h2><span class="icon">💡</span>The Philosophy</h2>
            <p>
                Web development isn't just a job for me—it's a passion. Every project is an opportunity to create something remarkable, to solve problems creatively, and to push the boundaries of what's possible on the web.
            </p>
            
            <h3>I Believe That</h3>
            <ul>
                <li><strong>The internet is humanity's greatest tool for communication</strong></li>
                <li><strong>Web development is the gateway to infinite possibilities</strong></li>
                <li><strong>Great technology should be accessible to everyone</strong></li>
                <li><strong>Continuous learning is the foundation of success</strong></li>
            </ul>
        </section>
 
        <hr>
 
        <!-- Let's Connect -->
        <section>
            <h2><span class="icon">🤝</span>Let's Connect</h2>
            <p>I'm always excited to:</p>
            <ul>
                <li>Collaborate on interesting projects</li>
                <li>Discuss web development trends</li>
                <li>Share knowledge and experiences</li>
                <li>Contribute to the developer community</li>
                <li>Explore new ideas together</li>
            </ul>
        </section>
 
        <hr>
 
        <!-- Quick Links -->
        <section>
            <h2><span class="icon">📚</span>Quick Links</h2>
            <div class="links-grid">
                <a href="#" class="link-card">💼 Portfolio (Coming Soon)</a>
                <a href="mailto:your-email@example.com" class="link-card">📧 Email Me</a>
                <a href="#" class="link-card">💬 LinkedIn</a>
                <a href="#" class="link-card">🐙 GitHub</a>
            </div>
        </section>
 
        <hr>
 
        <!-- Footer -->
        <footer>
            <p><strong>Let's build something extraordinary together.</strong> 🚀</p>
            <p>Last updated: April 2026 | Always learning, always growing</p>
            <p style="margin-top: 20px; font-size: 0.9rem;">
                This README represents my commitment to growth, excellence, and making a positive impact in the world of web development.
            </p>
        </footer>
    </div>
</body>
</html>

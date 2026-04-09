<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trungdoublelift - README</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
 
        :root {
            --primary: #0ea5e9;
            --accent: #f59e0b;
            --dark: #1e293b;
            --light: #f1f5f9;
            --bg: #ffffff;
            --text: #1e293b;
            --text-light: #64748b;
            --border: #e2e8f0;
            --code-bg: #f8fafc;
        }
 
        @media (prefers-color-scheme: dark) {
            :root {
                --bg: #0f172a;
                --text: #f1f5f9;
                --text-light: #cbd5e1;
                --border: #334155;
                --code-bg: #1e293b;
            }
        }
 
        html, body {
            height: 100%;
        }
 
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            background: var(--bg);
            color: var(--text);
            line-height: 1.6;
        }
 
        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 40px 20px;
        }
 
        h1 {
            font-size: 2.5em;
            margin: 1.2em 0 0.5em 0;
            color: var(--text);
            border-bottom: 1px solid var(--border);
            padding-bottom: 0.3em;
        }
 
        h2 {
            font-size: 1.8em;
            margin: 1.5em 0 0.5em 0;
            color: var(--text);
        }
 
        h3 {
            font-size: 1.3em;
            margin: 1.2em 0 0.5em 0;
            color: var(--text);
        }
 
        p {
            margin: 1em 0;
            line-height: 1.8;
            color: var(--text);
        }
 
        strong {
            color: var(--text);
            font-weight: 600;
        }
 
        em {
            color: var(--text-light);
            font-style: italic;
        }
 
        a {
            color: var(--primary);
            text-decoration: none;
            transition: color 0.3s ease;
        }
 
        a:hover {
            color: var(--accent);
            text-decoration: underline;
        }
 
        /* Blockquote / Quote */
        blockquote {
            background: rgba(14, 165, 233, 0.1);
            border-left: 4px solid var(--primary);
            padding: 1em 1.5em;
            margin: 1.5em 0;
            border-radius: 4px;
            font-style: italic;
            color: var(--text);
        }
 
        blockquote p {
            margin: 0.5em 0;
        }
 
        /* Horizontal Rule */
        hr {
            border: none;
            height: 2px;
            background: linear-gradient(90deg, transparent, var(--border), transparent);
            margin: 2.5em 0;
        }
 
        /* Lists */
        ul, ol {
            margin: 1.5em 0;
            padding-left: 2em;
            color: var(--text);
        }
 
        li {
            margin: 0.8em 0;
            line-height: 1.8;
            color: var(--text);
        }
 
        li strong {
            display: inline;
            color: var(--primary);
            font-weight: 600;
        }
 
        /* Code */
        code {
            background: var(--code-bg);
            padding: 0.2em 0.4em;
            border-radius: 3px;
            font-family: 'Courier New', monospace;
            font-size: 0.9em;
            color: var(--primary);
        }
 
        pre {
            background: var(--code-bg);
            border: 1px solid var(--border);
            padding: 1.5em;
            border-radius: 4px;
            overflow-x: auto;
            margin: 1.5em 0;
            font-family: 'Courier New', monospace;
            font-size: 0.9em;
            line-height: 1.4;
            color: var(--text);
        }
 
        pre code {
            background: transparent;
            padding: 0;
            color: var(--text);
        }
 
        /* Table */
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 1.5em 0;
            border: 1px solid var(--border);
            border-radius: 4px;
            overflow: hidden;
        }
 
        th {
            background: rgba(14, 165, 233, 0.1);
            color: var(--text);
            padding: 1em;
            text-align: left;
            font-weight: 600;
            border-bottom: 2px solid var(--border);
        }
 
        td {
            padding: 1em;
            border-bottom: 1px solid var(--border);
            color: var(--text);
        }
 
        tr:last-child td {
            border-bottom: none;
        }
 
        td strong {
            color: var(--primary);
        }
 
        /* Utility Classes */
        .text-muted {
            color: var(--text-light);
        }
 
        .highlight {
            color: var(--primary);
            font-weight: 600;
        }
 
        @media (max-width: 768px) {
            .container {
                padding: 20px 15px;
            }
 
            h1 {
                font-size: 2em;
            }
 
            h2 {
                font-size: 1.5em;
            }
 
            h3 {
                font-size: 1.1em;
            }
 
            table {
                font-size: 0.9em;
            }
 
            th, td {
                padding: 0.8em;
            }
 
            pre {
                font-size: 0.85em;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>👋 I'm <strong>Trungdoublelift</strong></h1>
 
        <blockquote>
            <p><em>"The only way to do great work is to love what you do."</em> – Steve Jobs</p>
        </blockquote>
 
        <p>Welcome to my corner of the internet. I'm a passionate developer on a mission to shape the future of web development and create meaningful digital experiences.</p>
 
        <hr>
 
        <h2>🌱 What I'm About</h2>
 
        <p>I'm currently deep in the world of <strong>Java</strong> and <strong>web development</strong>, constantly pushing boundaries and exploring innovative solutions. I believe the internet is the future of communication, and web development is the key to unlocking its potential.</p>
 
        <p>Every line of code I write is a step toward building something that matters—something that connects, inspires, and creates value for people around the world.</p>
 
        <hr>
 
        <h2>🚀 My Vision</h2>
 
        <p>The internet has revolutionized how we communicate. It's torn down geographical barriers, democratized information, and created endless possibilities for human connection. I'm committed to being at the forefront of this revolution.</p>
 
        <h3>Why I Do What I Do</h3>
 
        <ul>
            <li><strong>Innovation First</strong> — I believe in staying ahead of the curve, constantly learning and adapting to emerging technologies</li>
            <li><strong>Quality Over Quick</strong> — I write code that's clean, maintainable, and built to last</li>
            <li><strong>Impact Driven</strong> — Every project should solve a real problem and create genuine value</li>
            <li><strong>Continuous Growth</strong> — The moment I stop learning is the moment I stop growing</li>
        </ul>
 
        <hr>
 
        <h2>💻 Current Tech Focus</h2>
 
        <pre><code>Java              ████████████░░░░░░░░  85%
Web Development   ██████████████░░░░░░░  75%
Frontend          ███████████░░░░░░░░░░  65%
Backend           ████████████░░░░░░░░░  70%</code></pre>
 
        <p><strong>Learning & Exploring:</strong></p>
        <ul>
            <li>Advanced Java patterns and frameworks</li>
            <li>Modern web development practices</li>
            <li>Full-stack application development</li>
            <li>Performance optimization</li>
            <li>Cloud-native technologies</li>
        </ul>
 
        <hr>
 
        <h2>🎯 Core Values</h2>
 
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
 
        <hr>
 
        <h2>🌟 Key Beliefs</h2>
 
        <ul>
            <li>The best developers are lifelong learners</li>
            <li>Simplicity is the ultimate sophistication</li>
            <li>Community thrives on shared knowledge</li>
            <li>Great code is readable code</li>
            <li>Technology should serve humanity</li>
        </ul>
 
        <hr>
 
        <h2>📈 My Journey</h2>
 
        <p>I'm on an exciting journey of growth and discovery. Every day brings new challenges to solve, new technologies to explore, and new opportunities to make a difference.</p>
 
        <p><strong>What drives me:</strong></p>
        <ul>
            <li>Solving complex problems with elegant solutions</li>
            <li>Building scalable, maintainable applications</li>
            <li>Contributing to the open-source community</li>
            <li>Mentoring and learning from others</li>
            <li>Creating tools that improve people's lives</li>
        </ul>
 
        <hr>
 
        <h2>🔥 What's Next</h2>
 
        <p>I'm constantly evolving. Here's what's on my radar:</p>
 
        <ul>
            <li>✨ <strong>Mastering Java</strong> — Deep diving into enterprise-level Java development</li>
            <li>✨ <strong>Web Mastery</strong> — Becoming an expert in full-stack web development</li>
            <li>✨ <strong>Open Source</strong> — Contributing to meaningful projects</li>
            <li>✨ <strong>Building</strong> — Creating applications that make a real difference</li>
            <li>✨ <strong>Teaching</strong> — Sharing knowledge with the next generation of developers</li>
        </ul>
 
        <hr>
 
        <h2>💡 The Philosophy</h2>
 
        <p>Web development isn't just a job for me—it's a passion. Every project is an opportunity to create something remarkable, to solve problems creatively, and to push the boundaries of what's possible on the web.</p>
 
        <p>I believe that:</p>
        <ul>
            <li><strong>The internet is humanity's greatest tool for communication</strong></li>
            <li><strong>Web development is the gateway to infinite possibilities</strong></li>
            <li><strong>Great technology should be accessible to everyone</strong></li>
            <li><strong>Continuous learning is the foundation of success</strong></li>
        </ul>
 
        <hr>
 
        <h2>🤝 Let's Connect</h2>
 
        <p>I'm always excited to:</p>
        <ul>
            <li>Collaborate on interesting projects</li>
            <li>Discuss web development trends</li>
            <li>Share knowledge and experiences</li>
            <li>Contribute to the developer community</li>
            <li>Explore new ideas together</li>
        </ul>
 
        <hr>
 
        <h2>📚 Inspiration</h2>
 
        <p>This README represents my commitment to growth, excellence, and making a positive impact in the world of web development. Every day is a chance to get better, to learn something new, and to build something that matters.</p>
 
        <hr>
 
        <p><strong>Let's build something extraordinary together.</strong> 🚀</p>
 
        <p><em>Last updated: April 2026 | Always learning, always growing</em></p>
 
        <hr>
 
        <h3>Quick Links</h3>
        <ul>
            <li>💼 <a href="#">Portfolio</a> — Coming soon</li>
            <li>📧 Email — <a href="mailto:your-email@example.com">your-email@example.com</a></li>
            <li>💬 <a href="#">LinkedIn</a> — Connect with me</li>
            <li>🐙 <a href="#">GitHub</a> — Check out my code</li>
        </ul>
    </div>
</body>
</html>

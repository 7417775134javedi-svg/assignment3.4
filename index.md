Here is the complete code and structure for your assignment (Assignment 3.4 — Semantic HTML & Accessibility).

This file converts a traditional, non-semantic div-based layout into a fully compliant semantic HTML structure utilizing <header>, <nav>, <main>, <article>, <section>, <aside>, and <footer> tags, along with correct heading hierarchy and accessible image descriptions (alt text).

File: semantic-page.html
Save this code into a file named semantic-page.html:

HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TechInsights — Semantic HTML & Accessibility</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f4f6f8;
            color: #333;
        }
        header {
            background-color: #2c3e50;
            color: #ffffff;
            padding: 1.5rem 2rem;
            text-align: center;
        }
        nav {
            background-color: #34495e;
            display: flex;
            justify-content: center;
            padding: 0.75rem;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
        }
        nav a:hover {
            text-decoration: underline;
        }
        .container {
            display: flex;
            max-width: 1100px;
            margin: 2rem auto;
            gap: 2rem;
            padding: 0 1rem;
        }
        main {
            flex: 3;
        }
        article {
            background: white;
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
            margin-bottom: 2rem;
        }
        figure {
            margin: 1.5rem 0;
            text-align: center;
        }
        figure img {
            max-width: 100%;
            height: auto;
            border-radius: 4px;
        }
        figcaption {
            font-size: 0.9rem;
            color: #666;
            margin-top: 0.5rem;
        }
        section {
            background: white;
            padding: 1.5rem 2rem;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
        }
        aside {
            flex: 1;
            background: white;
            padding: 1.5rem;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
            height: fit-content;
        }
        aside ul {
            padding-left: 20px;
        }
        footer {
            text-align: center;
            padding: 1.5rem;
            background-color: #2c3e50;
            color: white;
            margin-top: 2rem;
        }
        h1, h2, h3 {
            color: #2c3e50;
        }
    </style>
</head>
<body>

    <!-- 1 & 2. Header and Navigation Elements -->
    <header>
        <h1>TechInsights</h1>
        <p>Your daily resource for modern web standards and accessibility practices.</p>
    </header>

    <nav aria-label="Main Navigation">
        <a href="#home">Home</a>
        <a href="#articles">Articles</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
    </nav>

    <!-- 3. Main Content Wrapper -->
    <div class="container">
        <main>
            <!-- Article Element for Independent Blog Post Content -->
            <article>
                <h2>The Importance of Semantic HTML in Modern Web Development</h2>
                <p>Published on <time datetime="2026-06-06">June 6, 2026</time> by Jane Doe</p>
                
                <p>Semantic HTML introduces clear meaning to web pages rather than just raw presentation. Using structural elements like <code>&lt;header&gt;</code>, <code>&lt;nav&gt;</code>, <code>&lt;main&gt;</code>, <code>&lt;article&gt;</code>, and <code>&lt;aside&gt;</code> helps screen readers, search engines, and developers understand page hierarchy instantly.</p>
                
                <!-- 5. Meaningful alt text for images -->
                <figure>
                    <img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c?auto=format&fit=crop&w=800&q=80" alt="A software developer sitting at a desk working on a laptop displaying lines of computer code in a dark text editor.">
                    <figcaption>Clean, well-structured code improves maintainability and accessibility.</figcaption>
                </figure>

                <h3>Why Accessibility Matters</h3>
                <p>When websites are built using generic <code>&lt;div&gt;</code> tags exclusively, assistive technologies struggle to distinguish navigation menus from main articles. Proper semantic landmarks solve this issue seamlessly.</p>
            </article>

            <!-- Section Element for Grouped Content -->
            <section>
                <h2>Related Topics</h2>
                <p>Explore further guides covering ARIA roles, responsive grid layouts, and cross-browser testing.</p>
            </section>
        </main>

        <!-- Aside Element for Sidebar / Secondary Information -->
        <aside>
            <h3>About the Author</h3>
            <p>Jane Doe is a front-end engineer and web accessibility advocate dedicated to building inclusive digital experiences.</p>
            
            <h3>Recent Posts</h3>
            <ul>
                <li><a href="#">Understanding ARIA Landmarks</a></li>
                <li><a href="#">CSS Flexbox vs CSS Grid</a></li>
                <li><a href="#">Optimizing Images for Performance</a></li>
            </ul>
        </aside>
    </div>

    <!-- Footer Element -->
    <footer>
        <p>&copy; 2026 TechInsights. All rights reserved.</p>
    </footer>

</body>
</html>
How to Complete Your Submission:
Save the File: Save the code above as semantic-page.html.

Review the Semantic Enhancements:

&lt;header&gt; & &lt;nav&gt;: Used for site introduction and clear navigation links.

&lt;main&gt;: Wraps the primary content container of the document.

&lt;article&gt; & &lt;section&gt;: Structures standalone content and related content groupings logically.

&lt;aside&gt;: Holds sidebar content like author information and related links.

Heading Hierarchy: Follows a clean structure (<h1> for title, <h2> for major block titles, <h3> for subheadings).

Accessibility (alt text): The image includes a descriptive alt attribute explaining what is visible for screen reader users.

Take Screenshots:

Before Screenshot: If you have an older non-semantic version of the file, take a screenshot of that code or page.

After Screenshot: Open your newly saved semantic-page.html in your web browser and take a screenshot showing the rendered semantic webpage.

Submit: Turn in your updated semantic-page.html file alongside your before and after screenshots.
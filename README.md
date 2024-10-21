# Emobilis-First-assignment
This is a  user-friendly form which contains a  personal portfolio landing page to showcase someone's skills and hobbies, with a separate contact page for potential connections.

### 1. Create the `index.html` file:

This file will be the entry point of your portfolio.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mary's Portfolio</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <style>
        /* Custom CSS for styling */
        body {
            font-family: Arial, sans-serif;
        }
        header {
            text-align: center;
            padding: 50px;
            background-color: #f8f9fa;
        }
        .tagline {
            text-align: center;
            margin: 30px 0;
        }
        #skills-hobbies {
            padding: 50px;
        }
        footer {
            text-align: center;
            padding: 20px;
            background-color: #343a40;
            color: white;
        }
        a {
            color: white;
        }
    </style>
</head>
<body>

    <!-- Navigation bar -->
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <a class="navbar-brand" href="#">Mary's Portfolio</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ml-auto">
                <li class="nav-item">
                    <a class="nav-link" href="#skills-hobbies">About Me</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="public/contact.html">Contact Me</a>
                </li>
            </ul>
        </div>
    </nav>

    <!-- Header Section -->
    <header>
        <img src="your-photo.jpg" alt="Your photo" class="img-fluid rounded-circle" style="width: 150px;">
        <h1>Mary - Electrician and Technology Enthusiast</h1>
    </header>

    <!-- Tagline Section -->
    <section class="tagline">
        <p>Bringing electrical projects to life with precision and creativity.</p>
    </section>

    <!-- Skills and Hobbies Section -->
    <section id="skills-hobbies" class="container">
        <div class="row">
            <div class="col-md-6">
                <h2>Skills</h2>
                <ul>
                    <li>Electrical wiring</li>
                    <li>Smart home installations</li>
                    <li>Electrical system maintenance</li>
                    <li>Problem-solving and troubleshooting</li>
                </ul>
            </div>
            <div class="col-md-6">
                <h2>Hobbies</h2>
                <ul>
                    <li>Learning computer science</li>
                    <li>Exploring renewable energy</li>
                    <li>DIY electronics projects</li>
                    <li>Hiking and outdoor adventures</li>
                </ul>
            </div>
        </div>
    </section>

    <!-- Footer Section -->
    <footer>
        <p>Connect with me on:</p>
        <a href="https://linkedin.com">LinkedIn</a> |
        <a href="https://github.com">GitHub</a> |
        <a href="mailto:youremail@example.com">Email</a>
    </footer>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.9.2/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>
```

### 2. Create the `contact.html` file:

This file will serve as the contact page inside a folder called `public`.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Me</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
</head>
<body>

    <!-- Navigation bar -->
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <a class="navbar-brand" href="../index.html">Mary's Portfolio</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav ml-auto">
                <li class="nav-item">
                    <a class="nav-link" href="../index.html#skills-hobbies">About Me</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="contact.html">Contact Me</a>
                </li>
            </ul>
        </div>
    </nav>

    <!-- Contact Form -->
    <div class="container">
        <h2>Contact Me</h2>
        <form>
            <div class="form-group">
                <label for="name">Name</label>
                <input type="text" class="form-control" id="name" placeholder="Your Name">
            </div>
            <div class="form-group">
                <label for="email">Email address</label>
                <input type="email" class="form-control" id="email" placeholder="Your Email">
            </div>
            <div class="form-group">
                <label for="phone">Phone Number</label>
                <input type="tel" class="form-control" id="phone" placeholder="Your Phone Number">
            </div>
            <div class="form-group">
                <label for="message">Message</label>
                <textarea class="form-control" id="message" rows="5" placeholder="Your Message"></textarea>
            </div>
            <button type="submit" class="btn btn-primary">Send</button>
        </form>
    </div>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.9.2/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>
```

### 3. Explanation of Features:

1. **Navbar**: Both pages have a navigation bar that links to the "About Me" section on the main page and the contact page.
2. **Responsive Layout**: The landing page uses Bootstrap's grid system to display a header, tagline, and a two-column layout for skills and hobbies.
3. **Linking to Sections**: The `About Me` link in the navbar smoothly scrolls to the "Skills and Hobbies" section using the `id="skills-hobbies"` attribute.
4. **Contact Page**: A simple form is provided for users to submit their name, email, phone number, and message.

This is a solid base that you can further customize with your unique content and styling.

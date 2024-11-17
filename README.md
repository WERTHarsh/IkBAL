
/* Main Styling */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f7f7f7; /* Light background */
    line-height: 1.6;
}

/* Tab Menu Styling */
.tab-menu {
    background-color: #3f51b5; /* Indigo for header menu */
    display: flex;
    justify-content: center;
    padding: 10px 0;
}

.tablink {
    color: #fff;
    padding: 10px 20px;
    font-size: 1em;
    font-weight: bold;
    text-decoration: none;
    margin: 0 5px;
    border-radius: 5px;
}

.tablink:hover {
    background-color: #5c6bc0; /* Lighter indigo on hover */
}

/* Section Styling with Different Colors */
.section-content {
    display: none; /* Hide all sections by default */
    padding: 30px;
    border-radius: 10px;
    margin: 20px auto;
    max-width: 900px;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
}

/* Home Section - Light Blue */
#home {
    background-color: #e3f2fd; /* Light blue background */
    color: #1e88e5; /* Blue text color */
}

/* About Me Section - Light Pink */
#about {
    background-color: #fce4ec; /* Light pink background */
    color: #e91e63; /* Pink text color */
}

/* My Favorite Things Section - Light Yellow */
#favorites {
    background-color: #fff9c4; /* Light yellow background */
    color: #fbc02d; /* Yellow text color */
}

/* Fun Projects Section - Light Purple */
#projects {
    background-color: #f3e5f5; /* Light purple background */
    color: #8e24aa; /* Purple text color */
}

/* Contact Section - Light Green */
#contact {
    background-color: #e8f5e9; /* Light green background */
    color: #43a047; /* Green text color */
}

/* Ensure Sections Displayed when Targeted */
#home:target, #about:target, #favorites:target, #projects:target, #contact:target {
    display: block; /* Show section when selected */
}

/* Default to show Home section */
body:not(:has(:target)) #home {
    display: block;
}

/* Heading Styling */
h1 {
    font-family: 'Georgia', serif;
    font-size: 2.5em;
    color: #3f51b5; /* Indigo color for main heading */
    text-align: center;
    margin-top: 20px;
}

h2 {
    font-family: 'Verdana', sans-serif;
    font-size: 1.8em;
    text-align: center;
    margin-bottom: 10px;
}

/* Content Styling */
p, ul {
    font-family: 'Tahoma', sans-serif;
    font-size: 1em;
    text-align: center;
    max-width: 800px;
    margin: auto;
    padding: 0 10px;
    font-style: italic;
}

ul {
    list-style-type: none;
    padding: 0;
}

li {
    margin: 10px 0;
}

/* Link Styling */
a {
    color: #3f51b5; /* Indigo color for links */
    text-decoration: none;
    font-weight: bold;
}

a:hover {
    text-decoration: underline;
    color: #5c6bc0; /* Lighter indigo on hover */
}

/* Image Styling */
.section-image {
    display: block;
    max-width: 100%; /* Ensure image fits within its container's width */
    max-height: 400px; /* Limit height, adjust as needed for your layout */
    width: auto;
    height: auto;
    margin: auto;
    border-radius: 10px; /* Rounded corners for aesthetics */
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
    object-fit: cover; /* Ensures images cover the area without distortion */
}

/* Contact Email Link Styling for Better Visibility */
.email-link {
    color: #004d40; /* Teal color for the email link */
    font-weight: bold;
}

.email-link:hover {
    color: #ff5722; /* Orange for hover effect on email link */
    text-decoration: underline;
}

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Fun Website</title>
    <link rel="stylesheet" href="style.css">
    <script defer src="script.js"></script>
    <style>
        /* Basic styles for different greetings */
        .morning {
            background-color: lightyellow;
            color: darkblue;
        }
        .afternoon {
            background-color: lightblue;
            color: darkgreen;
        }
        .evening {
            background-color: darkblue;
            color: white;
        }
    </style>
</head>
<body>

<!-- Tab Menu -->
<nav class="tab-menu">
    <a href="#home" class="tablink">Home</a>
    <a href="#about" class="tablink">About Me</a>
    <a href="#favorites" class="tablink">My Favorite Things</a>
    <a href="#projects" class="tablink">Fun Projects</a>
    <a href="#contact" class="tablink">Contact</a>
</nav>

<!-- Home Section -->
<section id="home" class="section-content">
    <h1>Welcome to My Fun Website!</h1>
    <img src="my_home.jpg" alt="Home Image" class="section-image">
    <p>This is a fun website where you can learn all about me, my favorite things, and the fun projects I do!</p>
    <div id="greeting"></div> <!-- Greeting will be displayed here -->
</section>

<!-- About Me Section -->
<section id="about" class="section-content">
    <h2>About Me</h2>
    <img src="about_image.jpg" alt="About Me Image" class="section-image">
    <p>Hi! My name is Heli Patel. I am 21 years old and I love to watch movies and do different circular activities. I enjoy spending time with my family and friends.</p>
</section>

<!-- My Favorite Things Section -->
<section id="favorites" class="section-content">
    <h2>My Favorite Things</h2>
    <img src="favorites_image.jpg" alt="Favorite Things Image" class="section-image">
    <ul>
        <li><strong>Favorite Toy:</strong> Lego Blocks</li>
        <li><strong>Favorite Color:</strong> Black</li>
        <li><strong>Favorite Game:</strong> Video games</li>
    </ul>
</section>

<!-- Fun Projects Section -->
<section id="projects" class="section-content">
    <h2>Fun Projects</h2>
    <img src="projects_image.jpg" alt="Fun Projects Image" class="section-image">
    <ul>
        <li><strong>Drawing and Coloring:</strong> I love drawing animals and nature.</li>
        <li><strong>Building with Blocks:</strong> I enjoy creating tall towers with my Lego blocks.</li>
        <li><strong>Making Crafts:</strong> I make fun crafts with paper, glue, and glitter.</li>
    </ul>
    <h3>Click the button below:</h3>
    <button id="btn-alert">Click me!</button>
    <h3>Numbers List:</h3>
    <ol id="numbers"></ol> <!-- Ordered list will be populated here -->
</section>

<!-- Contact Section -->
<section id="contact" class="section-content">
    <h2>Contact</h2>
    <p>If you want to send me a message, <a href="mailto:your-email@example.com" class="email-link">please reach out via email</a>!</p>
</section>

<!-- Footer will be populated by JavaScript -->
<footer></footer>
// Footer with Current Year
const footer = document.createElement('footer');
const currentYear = new Date().getFullYear();
footer.innerHTML = `&copy; Your Name, ${currentYear}`;
document.body.appendChild(footer);
console.log(new Date().toString()); // Prints today's entire date to the console

// Portfolio Greeting
const greetingElement = document.getElementById('greeting');
const currentHour = new Date().getHours();
let greetingMessage;

if (currentHour < 12) {
    greetingMessage = "Good morning!";
    greetingElement.classList.add('morning');
} else if (currentHour < 17) {
    greetingMessage = "Good afternoon!";
    greetingElement.classList.add('afternoon');
} else {
    greetingMessage = "Good evening!";
    greetingElement.classList.add('evening');
}

greetingElement.innerText = greetingMessage;

// Alert Button
const alertButton = document.getElementById('btn-alert');
alertButton.addEventListener('click', () => {
    alert("Hello world!");
});

// Hover Button
alertButton.onmouseover = function() {
    alertButton.innerText = "Hovered!";
};
alertButton.onmouseout = function() {
    alertButton.innerText = "Click me!";
};

// For Loop to Populate an Ordered List
const numbersList = document.getElementById('numbers');
for (let i = 1; i <= 12; i++) {
    const listItem = document.createElement('li');
    listItem.textContent = (i % 2 === 0) ? 'Even' : 'Odd';
    numbersList.appendChild(listItem);
}

</body>
</html>


<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link rel="stylesheet" href="style.css">
</head>
<body>
<header>
<h1>Our High School Girls Tennis Team</h1>
<nav>
<ul>
<li><a href="index.html">Home</a></li>
<li><a href="team.html">Team</a></li>
<li><a href="schedule.html">Schedule</a></li>
<li><a href="gallery.html">Gallery</a></li>
<li><a href="coaches.html">Coaches</a></li>
<li><a href="contact.html">Contact</a></li>
</ul>
</nav>
</header>
<main>

</main>
<footer>
<p>&copy; 2025 Our High School Girls Tennis Team</p>
</footer>
</body>
</html>


# Pages content

<h2>Welcome to the Girls Tennis Team Website!</h2>
<p>Here you’ll find everything you need to know about our team, including our match schedule, team members, photos, and how to get involved.</p>
<img src="tennis-team.jpg" alt="Girls Tennis Team Group Photo" />

<h2>Meet Our Team</h2>
<ul>
<li>Sophia — Team Captain</li>
<li>Emma</li>
<li>Olivia</li>
<li>Ava</li>
<li>Mia</li>
</ul>
<ul class="nested-list">
<li>Varsity Players
<ul>
<li>Sophia</li>
<li>Emma</li>
</ul>
</li>
<li>JV Players
<ul>
<li>Olivia</li>
<li>Ava</li>
<li>Mia</li>
</ul>
</li>
</ul>

<h2>Match & Practice Schedule</h2>
<table>
<thead>
<tr><th>Date</th><th>Opponent</th><th>Location</th><th>Time</th></tr>
</thead>
<tbody>
<tr><td>May 25</td><td>Lincoln High</td><td>Home</td><td>4:00 PM</td></tr>
<tr><td>May 28</td><td>Jefferson HS</td><td>Away</td><td>5:00 PM</td></tr>
</tbody>
</table>

<h2>Team Gallery</h2>
<figure>
<img src="match-action.jpg" alt="Action Shot from Last Match" />
<figcaption>Sophia serving during the final match.</figcaption>
</figure>
<figure>
<img src="practice.jpg" alt="Practice session" />
<figcaption>Team warming up before a match.</figcaption>
</figure>

<h2>Meet the Coaches</h2>
<p>Our team is led by Coach Taylor and Assistant Coach Morgan. Both have extensive tennis experience and are passionate about mentoring young athletes.</p>
<ul>
<li>Coach Taylor – Head Coach (10+ years experience)</li>
<li>Coach Morgan – Assistant Coach (former college player)</li>
</ul>

<h2>Contact Us</h2>
<form action="#" method="POST">
<label for="name">Name:</label>
<input type="text" id="name" name="name"><br>
<label for="email">Email:</label>
<input type="email" id="email" name="email"><br>
<label for="message">Message:</label><br>
<textarea id="message" name="message" rows="4"></textarea><br>
<input type="submit" value="Send">
</form>
<p>Watch our team in action:</p>
<video controls width="320">
<source src="team-highlight.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

}

# Create full HTML files
for filename, body in content.items():
with open(os.path.join(base_path, filename), 'w') as f:
f.write(header + body + footer)

# Write basic CSS for layout and accessibility
css_content = '''
body {
font-family: Arial, sans-serif;
margin: 0;
padding: 0;
background: #f8f8f8;
}
header, footer {
background-color: #003366;
color: white;
text-align: center;
padding: 1rem 0;
}
nav ul {
list-style: none;
padding: 0;
}
nav ul li {
display: inline-block;
margin: 0 10px;
}
nav ul li a {
color: white;
text-decoration: none;
}
main {
padding: 2rem;
}
table {
width: 100%;
border-collapse: collapse;
}
table, th, td {
border: 1px solid #ccc;
}
th, td {
padding: 10px;
text-align: center;
}
.nested-list ul {
list-style-type: circle;
margin-left: 20px;
}
form {
margin-top: 20px;
}
img, video {
max-width: 100%;
height: auto;
}
'''

with open(css_path, 'w') as f:
f.write(css_content)

base_path

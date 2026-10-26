## Assignment 6.5 — Profile Card Mini-Project

### 1. `index.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profile Card</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="profile-card">
        <span class="badge">Student</span>

        <img src="profile.jpg" alt="Profile photo" class="profile-image">

        <h1>Atul Kumar Pal</h1>
        <h3>B.Tech CSE Student</h3>

        <p>I am learning web development and programming.</p>

        <div class="skills">
            <span>HTML</span>
            <span>CSS</span>
            <span>Java</span>
        </div>

        <a href="mailto:atul@example.com" class="contact-button">
            Contact Me
        </a>
    </div>
</body>
</html>
```

### 2. `style.css`

```css
* {
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background: #eef2f7;
    margin: 0;
    padding: 30px;
}

.profile-card {
    position: relative;
    max-width: 350px;
    margin: 30px auto;
    padding: 25px;
    text-align: center;
    background: white;
    border: 1px solid #ddd;
    border-radius: 15px;
    box-shadow: 0 4px 12px #ccc;
}

.profile-image {
    width: 120px;
    height: 120px;
    border-radius: 50%;
    object-fit: cover;
    margin-top: 20px;
}

.badge {
    position: absolute;
    top: 12px;
    right: 12px;
    background: orange;
    padding: 6px 10px;
    border-radius: 10px;
}

h1 {
    color: navy;
    font-size: 24px;
}

.skills span {
    display: inline-block;
    background: #dce8f5;
    padding: 7px 12px;
    margin: 5px;
    border-radius: 5px;
}

.contact-button {
    display: inline-block;
    margin-top: 15px;
    padding: 10px 20px;
    background: navy;
    color: white;
    text-decoration: none;
    border-radius: 8px;
}

.contact-button:hover {
    background: royalblue;
}

@media (max-width: 400px) {
    body {
        padding: 10px;
    }

    .profile-card {
        padding: 18px;
    }
}
```

**Submission:** Save both files in the same folder and add your photo as `profile.jpg`. Open `index.html` with Live Server and take a screenshot. The card adjusts to smaller screens using a media query.
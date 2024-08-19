# day-12-task
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Design Example</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Responsive Web Page</h1>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Services</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section class="intro">
            <h2>Welcome to Our Website</h2>
            <p>This is an example of a responsive web design using HTML and CSS.</p>
        </section>
        <section class="content">
            <div class="box">Content Box 1</div>
            <div class="box">Content Box 2</div>
            <div class="box">Content Box 3</div>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Responsive Web Design</p>
    </footer>
</body>
</html>
/* Basic Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Typography */
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
}

/* Header */
header {
    background: #333;
    color: #fff;
    padding: 1em 0;
    text-align: center;
}

header nav ul {
    list-style-type: none;
}

header nav ul li {
    display: inline;
    margin: 0 10px;
}

header nav ul li a {
    color: #fff;
    text-decoration: none;
}

/* Main Content */
main {
    padding: 1em;
}

.intro {
    text-align: center;
    margin-bottom: 2em;
}

.content {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.box {
    background: #f4f4f4;
    padding: 20px;
    flex: 1 1 calc(33.333% - 20px);
    margin: 10px;
}

/* Footer */
footer {
    background: #333;
    color: #fff;
    text-align: center;
    padding: 1em 0;
    margin-top: 2em;
}

/* Responsive Design with Media Queries */
@media (max-width: 768px) {
    .content {
        flex-direction: column;
    }

    .box {
        flex: 1 1 100%;
        margin-bottom: 10px;
    }
}

@media (max-width: 480px) {
    header nav ul li {
        display: block;
        margin: 10px 0;
    }
}

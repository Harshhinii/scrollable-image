# scrollable-image
DATE:22-03-2025

# AIM : Design and implement an interactive image gallery using JavaScript, HTML, and CSS. The gallery should meet the following requirements:

 TASK : Display multiple images in a horizontal scrollable layout. Each image must have a caption that appears when hovered over. Include Next and Previous buttons to navigate through the images. Use JavaScript to enhance interactivity (e.g., smooth sliding animations, hover effects). Style the gallery using CSS for a visually appealing and responsive design. Include a footer at the bottom of the page with the text "Learner's Name and Register Number". Your solution should include well-structured HTML, CSS, and JavaScript code, ensuring smooth user experience and navigation.

# algorithm 

STEP 1
Create an HTML file (index.html)

STEP 2
Create a CSS file (style.css)

STEP 3
Create a JS file (script.js)

STEP 3
Include a navigation bar with links to different sections.

STEP 5
Define global styles for fonts, colors, and layout.

STEP 6
Style the Gallery, image, and footer.

STEP 7
Use CSS Grid for layout design.

STEP 8
Add hover effects and transitions for interactivity.

STEP 9
Add Images and Media.

STEP 10
Use optimized images for a professional look.

STEP 11
Open the HTML file in a browser to check layout and functionality.

STEP 12
Fix styling issues and refine content placement.

STEP 13
Deploy the Portfolio.

STEP 14
Upload to GitHub Pages for free hosting.
# PROGRAM
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Art Gallery</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Explore the Art Gallery</h1>
    <div class="gallery-container">
        <button id="prev">&#10094;</button>
        <div class="gallery">
            <div class="image-wrapper">
                <img src="art 1.jpg" alt="Art 1">
                <div class="caption">Mystic Mountains</div>
            </div>
            <div class="image-wrapper">
                <img src="art 2.jpg" alt="Art 2">
                <div class="caption">Ocean Serenity</div>
            </div>
            <div class="image-wrapper">
                <img src="art 3.jpg" alt="Art 3">
                <div class="caption">Golden Sunrise</div>
            </div>
            <div class="image-wrapper">
                <img src="art 4.jpg" alt="Art 3">
                <div class="caption">art journey</div>
            </div>
        </div>
        <button id="next">&#10095;</button>
    </div>
    <footer> HARSHINI R | 212223220033 </footer>
    <script src="script.js"></script>
</body>
</html>
```
```
body {
    font-family: Arial, sans-serif;
    text-align: center;
    background-color: #f4f4f4;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

h1 {
    color: #333;
}

.gallery-container {
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    max-width: 80%;
    margin: auto;
    flex-grow: 1; 
}

.gallery {
    display: flex;
    overflow-x: scroll;
    scroll-behavior: smooth;
    width: 80%;
    padding: 10px;
    gap: 10px;
}

.image-wrapper {
    position: relative;
    flex: 0 0 auto;
}

.image-wrapper img {
    width: 300px;
    height: 200px;
    border-radius: 10px;
    transition: transform 0.3s ease;
}

.image-wrapper:hover img {
    transform: scale(1.1);
}

.caption {
    position: absolute;
    bottom: 10px;
    left: 50%;
    transform: translateX(-50%);
    background: rgba(0, 0, 0, 0.6);
    color: white;
    padding: 5px 10px;
    border-radius: 5px;
    opacity: 0;
    transition: opacity 0.3s ease;
}

.image-wrapper:hover .caption {
    opacity: 1;
}

button {
    background: #333;
    color: white;
    border: none;
    padding: 10px;
    cursor: pointer;
    font-size: 18px;
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
}

#prev {
    left: 0;
}

#next {
    right: 0;
}

footer {
    padding: 10px;
    background: #222;
    color: white;
    text-align: center;
    width: 100%;
    position: relative;
    bottom: 0;
}
h1 {
    color: #333;
    margin-top: 150px; 
}
```
```
const gallery = document.querySelector(".gallery");
const prev = document.getElementById("prev");
const next = document.getElementById("next");

prev.addEventListener("click", () => {
    gallery.scrollBy({ left: -300, behavior: "smooth" });
});

next.addEventListener("click", () => {
    gallery.scrollBy({ left: 300, behavior: "smooth" });
});
```
# OUTPUT
![image](https://github.com/user-attachments/assets/c20153bc-d17f-4f25-a67a-44bdcad38dd2)

![image](https://github.com/user-attachments/assets/27cc77bf-facf-45e3-8d0d-bbd2935250ad)

# RESULT
This experiment is implemented using HTML,CSS and JS.


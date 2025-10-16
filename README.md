# Ex.08 Design of Interactive Image Gallery
## Date:13/10/2025

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Image Gallery</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Image Gallery</h1>

    <div class="gallery">
        <img src="vijay.jpg" alt="VIJAY" onclick="openModal(this)">
        <img src="sk.jpg" alt="SIVAKARTHIKEYAN" onclick="openModal(this)">
        <img src="rajini.jpg" alt="RAJINIKANTH" onclick="openModal(this)">
        <img src="str.jpg" alt="SILAMBARASAN" onclick="openModal(this)">
        <img src="Dhanush.jpg" alt="DHANUSH" onclick="openModal(this)">
    </div>

    <footer>
        <h2>&copy; DESIGNED BY: Dhanyamala Gokul Kumar(25011343)</h2>
        
    </footer>

    <script src="script.js"></script>
</body>
</html>

style.css

body {
    font-family: Arial, sans-serif;
    background-color: rgb(118, 55, 55);
    text-align: center;
    margin: 0;
}

h1 {
    background-color: rgb(22, 9, 9);
    color: white;
    padding: 20px;
    margin: 10;
}

.gallery {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 5px;
    padding: 50px;
}

.gallery img {
    width: 240px;
    height: 400px;
    border-radius: 20px;
    cursor: pointer;
    transition: transform 0.5s, box-shadow 1.5s;
}

.gallery img:hover {
    transform: scale(1.05);
    box-shadow: 0 4px 10px rgba(28, 15, 15, 0.3);
}

/* Modal Styles */
.modal {
    display: none;
    position: fixed;
    z-index: 100;
    left: 0;
    top: 0;
    width: 50%;
    height: 60%;
    background-color: rgba(0,0,0,0.9);
}

.modal-content {
    display: block;
    margin: 5% auto;
    max-width: 80%;
    border-radius: 10px;
}

#caption {
    color: white;
    text-align: center;
    margin-top: 10px;
}

scripts.js

function openModal(img) {
    var modal = document.getElementById("modal");
    var modalImg = document.getElementById("modalImg");
    var caption = document.getElementById("caption");
    
    modal.style.display = "block";
    modalImg.src = img.src;
    caption.innerHTML = img.alt;
}

function closeModal() {
    document.getElementById("modal").style.display = "none";
}




```
## OUTPUT:
<img width="1907" height="798" alt="image" src="https://github.com/user-attachments/assets/58325766-3c3b-4162-a5ff-f37356dd18ad" />

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.

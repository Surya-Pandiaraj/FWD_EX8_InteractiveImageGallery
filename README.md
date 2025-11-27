### NAME: SURYA P <br>
### REG NO: 212224230280 <br> 
### Date: 13/11/2025

## EX. No. 8 : INTERACTIVE IMAGE GALLERY


## AIM :
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS :

## Step 1

Clone the github repository and create Django admin interface

## Step 2

Change settings.py file to allow request from all hosts.

## Step 3

Use CSS for positioning and styling.

## Step 4

Write JavaScript program for implementing interactivit

## Step 5

Validate the HTML and CSS code

## Step 6

Publish the website in the given URL.

## PROGRAM :

```html
<!DOCTYPE html>
<html>
<head>
    <title>Interactive Image Gallery</title>

<style>
    body {
        margin: 0;
        padding: 30px;
        font-family: Arial, sans-serif;
        background: linear-gradient(135deg, #f3f5f7, #4a67bc);
        text-align: center;
        color: white;
    }

    h1 {
        font-size: 150px;       
        margin-bottom: 20px;
    }

    h2 {
        font-size: 60px;       
        margin-top: 10px;
        margin-bottom: 50px;
    }

    .gallery {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 60px;
        margin-top: 50px;
    }

    .gallery img {
        height: 500px;
        width: 300px;
        border-radius: 14px;
        box-shadow: 0 6px 20px rgba(0,0,0,0.35);
        cursor: pointer;
        transition: transform 0.3s;
    }

    .gallery img:hover {
        transform: scale(1.08);
    }

    /* MODAL */
    .modal {
        display: none;
        position: fixed;
        z-index: 999;
        padding-top: 80px;
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(0,0,0,0.8);
    }

    .modal-content {
        margin: auto;
        display: block;
        max-width: 80%;
        border-radius: 12px;
        animation: zoom 0.4s ease-in-out;
    }

    @keyframes zoom {
        from {transform: scale(0.6);}
        to {transform: scale(1);}
    }

    #close {
        position: absolute;
        top: 30px;
        right: 40px;
        font-size: 45px;
        color: white;
        cursor: pointer;
        font-weight: bold;
    }

    footer {
        margin-top: 100px;
        font-size: 30px;
        font-weight: bold;
    }
</style>

</head>
<body>

<h1>GALLERY</h1>
<h2>Interactive Image Gallery</h2>

<div class="gallery">
    <img src="images/img1.jpg" alt="Image 1" onclick="openModal(this.src)">
    <img src="images/img2.jpg" alt="Image 2" onclick="openModal(this.src)">
    <img src="images/img3.jpg" alt="Image 3" onclick="openModal(this.src)">
    <img src="images/img4.jpg" alt="Image 4" onclick="openModal(this.src)">
    <img src="images/img5.jpg" alt="Image 5" onclick="openModal(this.src)">
    <img src="images/img6.jpg" alt="Image 6" onclick="openModal(this.src)">
</div>

<!-- MODAL -->
<div id="imgModal" class="modal">
    <span id="close" onclick="closeModal()">&times;</span>
    <img class="modal-content" id="modalImg">
</div>

<!-- JAVASCRIPT -->
<script>
    function openModal(src) {
        document.getElementById("imgModal").style.display = "block";
        document.getElementById("modalImg").src = src;
    }

    function closeModal() {
        document.getElementById("imgModal").style.display = "none";
    }
</script>

<footer>
    Designed and Developed by <b>Surya P (212224230280)</b>
</footer>

</body>
</html>

```

## OUTPUT :
<img width="1899" height="1019" alt="image" src="https://github.com/user-attachments/assets/ddecc117-8eee-4c6a-92a3-33905e46b1c7" />
<img width="1895" height="983" alt="image" src="https://github.com/user-attachments/assets/0df96075-86f0-4a18-8578-8da81b0f3be2" />


## RESULT :
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.

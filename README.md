# Ex.08 Design of Interactive Image Gallery
## Date:07-10-2025

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

pic.html

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gallery</title>
    <link rel="stylesheet"
        href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&family=Playfair+Display:wght@700&display=swap">
    <link rel="stylesheet" href="pic.css">
</head>

<body>
    <h1>MY GALLERY</h1 color=aqua>
    <div class="ref">
        <div class="main-items" ><img src="imagephoto.png" alt="MyPhoto"></div>
        <div class="main-items"><img src="IMG-20251007-WA0002.jpg"
                alt="SMRITHI MANDHANA"></div>
        <div class="main-items"><img
                src="IMG-20251007-WA0003.jpg"
                alt="ABD"></div>
        <div class="main-items"><img src="IMG-20251007-WA0004.jpg"
                alt="VIRAT KOHLI"></div>
        <div class="main-items"><img
                src="kl rahul.jpg"
                alt="KL RAHUL"></div>
    </div>
    <h2>&copy; ALBUM <br> <strong>SIVAPRASATH B - 25016007</strong></h2>
    <div id="modal" class="mod">
        <span class="close"></span>
        <img id="modalImg" class="modal-content">
    </div>
        <script>
             var modal = document.getElementById('modal');
        var modalImg = document.getElementById('modalImg');
        document.querySelectorAll('.main-items img').forEach(img =>
            img.onclick = () => {
                modal.style.display = 'block';
                modalImg.src = img.src;
            }
        );
        modal.addEventListener('click', (e) => {
            if (e.target === modal) {
                modal.style.display = 'none';
            }
        });
    </script>
    </body>
</html>


pic.css



* {
    padding: 0px;
    margin: 0px;
    box-sizing: border-box;
}

body {
    background-color: rgb(237, 19, 4);
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.main-items img {
    width: 300px;
    height: auto;
    cursor: pointer;
    padding: 25px;
    border-radius: 20%;
}

.mod {
    display: none;
    position: fixed;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(6, 141, 245, 0.9);
    padding-top: 60px;
}

.mod img {
    margin: auto;
    display: block;
    max-width: 80vw;
    max-height: 80vh;
}

.ref {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    margin-top: 150px;
    background-color: rgb(10, 10, 10);
    padding: 50px 0px 50px 0px;
}

.close {
    position: absolute;
    top: 15px;
    right: 35px;
    color: rgb(183, 93, 93);
    font-size: 40px;
    font-weight: bold;
    transition: 0.3s;
}


h2 {
    letter-spacing: normal;
    position: absolute;
    left: 7%;
    top:90%;
    color:aqua;
    font-family: inter;
}

```

## OUTPUT:

![alt text](<Screenshot 2025-10-07 210405.png>)

![alt text](<Screenshot 2025-10-07 210432.png>)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.

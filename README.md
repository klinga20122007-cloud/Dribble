# Project Responsive Web Design using Bootstrap
## Date:

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
```
index.html

{% load static %}

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dribbble Clone</title>

    <link rel="stylesheet" href="{% static 'style.css' %}">
</head>
<body>

    <nav>
        <div class="logo">Dribbble</div>

        <ul>
            <li>Shots</li>
            <li>Designers</li>
            <li>Teams</li>
        </ul>
    </nav>

    <div class="container">

        <div class="card">
            <img src="{% static 'img1.jpg' %}" alt="">
            
            <div class="content">
                <h3>Modern UI</h3>
                <p>4,000 Views</p>
            </div>
        </div>

        <div class="card">
            <img src="{% static 'img2.jpg' %}" alt="">
            
            <div class="content">
                <h3>Creative Design</h3>
                <p>2,500 Views</p>
            </div>
        </div>

        <div class="card">
            <img src="{% static 'img3.jpg' %}" alt="">
            
            <div class="content">
                <h3>Dashboard UI</h3>
                <p>5,000 Views</p>
            </div>
        </div>

    </div>

</body>
</html>

style.css

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial;
}

body{
    background:#f3f3f3;
}

nav{
    background:#111;
    color:white;
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:20px 60px;
}

.logo{
    font-size:28px;
    font-weight:bold;
}

nav ul{
    display:flex;
    gap:30px;
    list-style:none;
}

nav ul li{
    cursor:pointer;
}

.container{
    width:90%;
    margin:40px auto;

    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
    gap:30px;
}

.card{
    background:white;
    border-radius:12px;
    overflow:hidden;

    box-shadow:0 5px 15px rgba(0,0,0,0.1);

    transition:0.3s;
}

.card:hover{
    transform:translateY(-10px);
}

.card img{
    width:100%;
    height:250px;
    object-fit:cover;
}

.content{
    padding:20px;
}

.content h3{
    margin-bottom:10px;
}

.content p{
    color:gray;
}
``` 

## OUTPUT:
<img width="1913" height="958" alt="{454E06EC-0D01-46CD-BC38-6BE4AB6F8313}" src="https://github.com/user-attachments/assets/d552bbfa-d448-4627-b092-69090a0f2f6c" />

## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.

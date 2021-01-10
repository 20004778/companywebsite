# Web Design for a Manufacturing Company
## AIM: 
To design a static website for a chip manufacturing company.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Updating the sample content.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.

## PROGRAM:

### base.html
```
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Silicon Private Limited</title>
    <link rel="stylesheet" href="{% static 'css/layout.css' %}">
    <link rel="icon" href="{% static 'img/titla.png' %}" type="image/x-icon">

</head>

<body>
    <div class="container">
        <div class="banner">
            Silicon Private Limited
        </div>
        <div class="menu">
            <div class="menuitem"><a href="/home">Home</a></div>
            <div class="menuitem"><a href="/products">Products</a></div>
            <div class="menuitem"><a href="/people">People</a></div>
            <div class="menuitem"><a href="/contactus">ContactUs</a></div>
        </div>
        <div class="content">
            {% block content %}
            {% endblock  %}
        </div>
        <div class="footer">
            Copyright © 2021 Silicon Private Limited, Developed by surya.
        </div>
    </div>
</body>

</html>
```

### home.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="homecontent">    
    <h1>About Us</h1>
    <img src="/static/img/titla.png" alt="Building">
    <div class="contenttext">
    Silicon Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications that serve the data center, networking, software, broadband, wireless, and storage and industrial markets. Common applications for its products include: data center networking, home connectivity, broadband access, telecommunications equipment, smartphones, base stations, data center servers and storage, factory automation, power generation and alternative energy systems, displays, and mainframe operations and management, and application software development. Some of Silicon's core technologies and products include:
    <ul>
        <li> Memory Chips </li>
        <li> SATA HDD </li>
        <li> SATA SSD </li>
        <li> Broadband Modems </li>
        <li> Wifi Devices </li>
        <li> Switching Devices </li>
        <li> Optical Sensors </li>
    </ul> 
    </div>
    </div>
{% endblock  %}
```

### products.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="productcontent">
        <h1>Our Premium Products</h1>
        <div class="productitems">
            <div class="productitem">
                <div class="itemimage">
                    <img src="/static/img/HyperXFury8GB.jpg" alt="product image">
                </div>
                <div class="itemname">8GB hyperx laptop memory</div>
                <div class="itemprice">Price: Rs.10,000.00 </div>
            </div>
            <div class="productitem">
                <div class="itemimage">
                    <img src="/static/img/c2.jpg" alt="product image">
                </div>
                <div class="itemname">1TB Laptop HDD</div>
                <div class="itemprice">Price: Rs.5000.00 </div>
            </div>
            <div class="productitem">
                <div class="itemimage">
                    <img src="/static/img/ChiptronexGX3000RGB.jpg" alt="product image">
                </div>
                <div class="itemname">Chiptronex GX3000 RGB </div>
                <div class="itemprice">Price: Rs.1,100,00.00 </div>
            </div>
            <div class="productitem">
                <div class="itemimage">
                    <img src="/static/img/keyboard.jpg" alt="product image">
                </div>
                <div class="itemname"> E - Royal Shop Rainbow LED</div>
                <div class="itemprice">Price: Rs.899.00 </div>
            </div>
            <div class="productitem">
                <div class="itemimage">
                    <img src="/static/img/mouse.jpg" alt="product image">
                </div>
                <div class="itemname"> E - Royal mouse </div>
                <div class="itemprice">Price: Rs.300.00 </div>
            </div>
            <div class="productitem">
                <div class="itemimage">
                    <img src="/static/img/ram.jpg" alt="product image">
                </div>
                <div class="itemname"> DDR4 3200 MHz RAM for Desktop PC </div>
                <div class="itemprice">Price: Rs.3,400.00 </div>
            </div>
            <div class="productitem">
                <div class="itemimage">
                    <img src="/static/img/specker.jpg" alt="product image">
                </div>
                <div class="itemname"> Zebronics Zeb-Warrior 2.0 </div>
                <div class="itemprice">Price: Rs.300.00 </div>
            </div>
            <div class="productitem">
                <div class="itemimage">
                    <img src="/static/img/camera.jpg" alt="product image">
                </div>
                <div class="itemname">Zebronics Zeb-Crystal Clear Web Camera with 3P Lens </div>
                <div class="itemprice">Price: Rs.300.00 </div>
            </div>
            <div class="productitem">
                <div class="itemimage">
                    <img src="/static/img/motherboard.jpg" alt="product image">
                </div>
                <div class="itemname"> Dual 9P Motherboard Header Extension Cable </div>
                <div class="itemprice">Price: Rs.300.00 </div>
            </div>
            <div class="productitem">
                <div class="itemimage">
                    <img src="/static/img/htmlcable.jpg" alt="product image">
                </div>
                <div class="itemname">Converter Adapter Cable (Black)</div>
                <div class="itemprice">Price: Rs.200.00 </div>
            </div>
            <div class="productitem">
                <div class="itemimage">
                    <img src="/static/img/networkadopter.jpg" alt="product image">
                </div>
                <div class="itemname">TP-LINK TG-3468 Gigabit PCI Express Network Adapter</div>
                <div class="itemprice">Price: Rs.200.00 </div>
            </div>
            <div class="productitem">
                <div class="itemimage">
                    <img src="/static/img/fan.jpg" alt="product image">
                </div>
                <div class="itemname">Electronic Spices Electronicspices DC 12V HIGH END Cooling Fan Black for PC Case CPU
                    Cooler r</div>
                <div class="itemprice">Price: Rs.400.00 </div>
            </div>
        </div>    
    </div>
{% endblock  %
```

### people.html
```
{% extends "website/base.html" %}

{% block content %}
    <h1>S</h1>
    <div>
    <h2><b>ROBERT_DOWNEY JR</b></h2>
    <div class="itemimage">
        <img src="/static/img/robertdowneyjr.jpg" alt="executive image" width="250" height="300">
    </div>
    <P>Designation:<b>FOUNDER</b></P>
    </div>

    <div>
    <br>
    <h2><b>JACK_MA</b></h2>
    <div class="itemimage">
        <img src="/static/img/jackma.jpg" alt="executive image" width="250" height="300">
    </div>
    <P>Designation:<b>CEO</b></P>
    <br>
    </div>

    <div>
    <br>
    <h2><b>LARRY_ELLISON</b></h2>
    <div class="itemimage">
        <img src="/static/img/larryellison.jpg" alt="executive image" width="250" height="300">
    </div>
    <P>Designation:<b>TECHNICAL HEAD</b></P>
    <br>
    </div>

    <div>
    <br>
    <h2><b>GAUTAM_ADANI</b></h2>
    <div class="itemimage">
        <img src="/static/img/GautamAdani.jpg" alt="executive image" width="250" height="300">
    </div>
    <P>Designation:<b>R&D HEAD</b></P>
    <br>
    </div>

    <div>
    <br>
    <h2><b>CHRIS_HEMSWORTH</b></h2>
    <div class="itemimage">
        <img src="/static/img/chrishemsworth.jpg" alt="executive image" width="250" height="300">
    </div>
    <P>Designation:<b>DESIGN HEAD</b></P>
    <br>
    </div>

    <div>
    <br>
    <h2><b>GIGI_HADID</b></h2>
    <div class="itemimage">
        <img src="/static/img/gigihadid.jpg" alt="executive image" width="250" height="300">
    </div>
    <P>Designation:<b>MARKETTING HEAD</b></P>
    <br>
    </div>
{% endblock  %}
```

### contactus.html
```
{% extends "website/base.html" %}

{% block content %}
   <img src="/static/img/contact.jpg" alt="contact">

    <h1>
           CONTACT
    </h1>
    <hr>
    <h2>
           EMAIL ID:siliconprivatelimited@gmail.com<br>
            <br>
       CONTACT NO:9344857514
    </h2>
    <hr>
{% endblock  %
```

## OUTPUT:
![output](./static/img/home.jpg)
![output](./static/img/product.jpg)
![output](./static/img/people.jpg)
![output](./static/img/contactus.jpg)

## CODE VALIDATION REPORT:
![output](./static/img/home.val.jpg)
![output](./static/img/product.val.jpg)
![output](./static/img/people.val.jpg)
![output](./static/img/contactus.val.jpg)

## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://surya.student.saveetha.in:8000/. HTML code is validated.
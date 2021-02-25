# Dynamic Website Design for a Manufacturing Company
## AIM:
To design a dynamic website for a chip manufacturing company.

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
### Step 7:
Create a database model and migrate the database.
### Step 8:
Retrieve data from database and display it in a dynamic webpage.
### Step 9:
Publish the website in the given URL.

## PROGRAM:
### home. html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="homecontent">    
    <h1>About Us</h1>
    <img src="/static/img/build.jpg" alt="Building">
    <div class="contenttext">
    AR Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications that serve the data center, networking, software, broadband, wireless, and storage and industrial markets. Common applications for its products include: data center networking, home connectivity, broadband access, telecommunications equipment, smartphones, base stations, data center servers and storage, factory automation, power generation and alternative energy systems, displays, and mainframe operations and management, and application software development. Some of Silicon's core technologies and products include:
    <ul>
        <li>Memory Chips</li>
        <li>SATA HDD</li>
        <li>SATA SSD </li>
        <li>Broadband Modems</li>
        <li>Wifi Devices</li>
        <li>Switching Devices</li>
        <li>Optical Sensors</li>
    </ul> 
    </div>
    </div>
{% endblock  %}
```
### people.html
```
% extends "website/base.html" %}

{% block content %}
<div class="peoplecontent">
    <h1>Executives</h1>
    <div class="crewmembers">
        {% for people in peoples %}
        <div class="crewmember">
            <div class="memberimage">
                <img src="{{ people.photo.url }}" alt="member image" height="200" width="200">
            </div>
            <div class="Membername">{{ people.Membername }}</div>
            <div class="Designation">{{ people.Designation }}</div>
        </div>
        {% endfor %}
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
    {% for product in products  %}
        <div class="productitem"> 
            <div class="itemimage">
            <img src="{{ product.photo.url }}" alt="product image">
            </div>
            <div class="Itemname">Name:{{ product.Itemname }}</div>
            <div class="Product price">Price:{{ product.Price }}</div>
        </div>
    {% endfor %}
    </div>
{% endblock  %}

```
### contact.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="contactuscontent">
        <div class="contactbox">
            <div>
                <img src="/static/img/contact.png" alt="contactusimg">
            </div>
        </div>
        <hr/>
        <div class="contactemail"><h1>Email: arun@ar.ac.in</h1></div>
        <div class="contactphone"><h2>Phone: +91-7200742352</h2></div>
        <div class="contactphone"><h2>Address: © AR pvt,Silicon valley, Microsoft, Google</h2></div>
        <hr/>
    </div>

{% endblock %}

```
## OUTPUT:

## OUTPUT:
![output](./static/img/output/o1.png)

![output](./static/img/output/o2.png)

![output](./static/img/output/o3.png)

![output](./static/img/output/o4.png)

![output](./static/img/output/o4.png)

![output](./static/img/output/o4.png)

## CODE VALIDATION REPORT:
![output](./static/img/report/v1.png)

![output](./static/img/report/v2.png)

![output](./static/img/report/v3.png)


## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://arun.student.saveetha.in:8000/. HTML code is validated.

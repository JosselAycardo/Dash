<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Homepage</title>
    <link rel="stylesheet" href="Example.css">
</head>
<body>
    <div class="full-page">
        <div class="navbar">
            <div>
                <a href='Example.html'>Dental Clinic</a>
            </div>
            <nav>
                <ul id='MenuItems'>
                    <li><a href='Example.html'>Home</a></li>
                    <li class="services-item"><a href='#'>Services</a>
                        <div class="sub-menu">
                            <ul>
                                <li><a href='Rootcanal.html'>Root Canal</a></li>
                                <li><a href='check.html'>Check-up</a></li>
                                <li><a href='Crown.html'>Crown and Bridges</a></li>
                                <li><a href='Cleaning.html'>Cleaning</a></li>
                            </ul>
                        </div>
                    </li>
                    <li><a href='Contactus.html'>Contact Us</a></li>
                    <li><a href='booking.html'>Book Appointment</a></li>
                    <li><a href='Aboutus.html'>About Us</a></li>
                </ul>
            </nav>
        </div>
        
    </div>
</body>
</html>












css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

.full-page {
    height: 100%;
    width: 100%;
    background-image: linear-gradient(rgba(0,0,0,0.4),rgba(0,0,0,0.4)), url(clinic1.jpg);
    background-position: center;
    background-size: cover;
    position: absolute;
}

.navbar {
    display: flex;
    align-items: center;
    padding: 20px;
    padding-left: 50px;
    padding-right: 30px;
    padding-top: 50px;
}

nav {
    flex: 1;
    text-align: right;
}

nav ul {
    display: inline-block;
    list-style: none;
}

nav ul li {
    display: inline-block;
    margin-right: 70px;
    position: relative;
}

nav ul li a {
    text-decoration: none;
    font-size: 20px;
    color: rgb(255, 255, 255);
    font-family: sans-serif;
}

nav ul li button {
    font-size: 20px;
    color: white;
    outline: none;
    border: none;
    background: transparent;
    cursor: pointer;
    font-family: sans-serif;
}

nav ul li button:hover {
    color: aqua;
}
nav ul li a .book{
    color: rgb(255, 0, 0);
}
nav ul li a:hover {
    color: aqua;
}


a {
    text-decoration: none;
    color: rgb(0, 0, 0);
    font-size: 28px;
}

.button-box {
    width: 220px;
    margin: 35px auto;
    position: relative;
    box-shadow: 0 0 20px 9px #64646441;
    border-radius: 30px;
}

.toggle-btn {
    padding: 10px 30px;
    cursor: pointer;
    background: transparent;
    border: 0;
    outline: none;
    position: relative;
}

#btn {
    top: 0;
    left: 0;
    position: absolute;
    width: 110px;
    height: 100%;
    background: #ffb671d8;
    border-radius: 30px;
    transition: 0.5s;
}

.input-field {
    width: 100%;
    padding: 10px 0;
    margin: 5px 0;
    border-left: 0;
    border-top: 0;
    border-right: 0;
    border-bottom: 1px solid #00000065;
    outline: none;
    background: transparent;
}

.submit-btn {
    width: 85%;
    padding: 10px 30px;
    cursor: pointer;
    display: block;
    margin: auto;
    background: #ffb671d8;
    border: 0;
    outline: none;
    border-radius: 30px;
}

.check-box {
    margin: 30px 10px 34px 0;
}

span {
    color: #000000;
    font-size: 12px;
    bottom: 68px;
    position: absolute;
}

.sub-menu {
    display: none;
    position: absolute;
    background: #ffffff;
    margin-top: 0;
    margin-left: -15px;
    padding: 10px 0;
    transition: display 5s ease-in-out, opacity 5s ease-in-out;
    opacity: 0;
}
.sub-menu ul li:hover {
    color: rgb(255, 255, 255);
}
.services-item:hover .sub-menu {
    display: block;
    opacity: 1;
    transition-delay: 5s;
}

.services-item .sub-menu ul {
    display: none;
    position: absolute;
    background: #373b3b7c;
    margin-top: 0;
    margin-left: -15px;
    padding: 10px 0;
    transition: display 5s ease-in-out, opacity 5s ease-in-out;
    opacity: 0;
}

.services-item:hover .sub-menu ul {
    display: block;
    opacity: 1;
    transition-delay: 5s;
}

.services-item:hover .sub-menu ul li {
    width: 150px;
    padding: 10px;
    background: transparent;
    border-radius: 0;
    text-align: left;
}

.services-item:hover .sub-menu ul li:last-child {
    border-bottom: none;
}

.services-item:hover .sub-menu ul li:hover {
    color: #ffffff;
}

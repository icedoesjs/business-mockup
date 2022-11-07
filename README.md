# business-mockup

Ashley Fightmaster

Ashley's HTML:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://kit.fontawesome.com/9f93281985.js" crossorigin="anonymous"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@100;400;500;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="css/focusonyourbusiness.css">
    <title>Document</title>
</head>
<body>
<div class="left">
    <h1>Focus on <br> Your Business</h1> 
    <h3>Let Us Handle Everything Else</h3>
    <p id="description">Subscription Billing, powered with revenue retention tools and a seamless customer experience - without the technical hurdles. </p>
    <button class="button1" onclick="location.href='signup.html'" type="button"><span>Sign Up Now</span></button>  
    <button class="button2"><i class="fa-regular fa-comment-dots"></i> <span>Chat With Us
    </span></button>
    <p id="sign-in">Already using <strong>Dunder Mifflin</strong>? <a id="sign-in2"href="#">Sign In</a></p>
    <ul class="bottom">
        <li>Free 14 day trial <span class="dot"></span> </li>
        <li>Manage Paper in Minutes <span class="dot"></span></li>
        <li>Cancel at Anytime</li>
    </ul>
</div>
<div class="container">
    <button class="item1" onclick="location.href='#'" type ="button"><i class="fa-solid fa-grip"></i><span id="text">Client Dashboard</span></button>
    <button class="item2" onclick="location.href='#'" type ="button"><i class="fa-solid fa-chart-simple"></i><span id="text">Analytics</span></button>
    <button class="item3" onclick="location.href='#'" type ="button"><i class="fa-regular fa-clock"></i><span id="text">Tracking</span></button>
    <button class="item4" onclick="location.href='#'" type ="button"><i class="fa-regular fa-id-badge"></i><span id="text">Employee Profiles</span></button>
    <button class="item5" onclick="location.href='#'" type ="button"><i class="fa-solid fa-comments"></i><span id="text">Comments</span></button>
    <button class="item6" onclick="location.href='#'" type ="button"><i class="fa-solid fa-envelope-open"></i><span id="text">Email</span></button>
    <button class="item7" onclick="location.href='#'" type ="button"><i class="fa-solid fa-calendar-days"></i><span id="text">Client Calender</span></button>
    <button class="item8" onclick="location.href='#'" type ="button"><i class="fa-regular fa-folder-open"></i><span id="text">Project Folders</span></button>
    <button class="item9" onclick="location.href='#'" type ="button"><i class="fa-regular fa-bell"></i><span id="text">Project Alerts</span></button>
</div>
</body>
</html>

Ashley's CSS:
*{
    margin: 0px;
    padding: 0px;
    font-family: 'Roboto', sans-serif;
    cursor: default;
}

/* Responsive layout - makes a one column-layout instead of two-column layout */
@media (max-width: 800px) {
    .left, .container {
    flex-direction: column;
    }
}

.left{
    width:40%;
    padding: 5px;
    margin: 20px;
    display:flex;
    justify-content: center;
    flex-wrap: wrap;
    flex-direction: column;
    flex-grow: 0;
}

h3{
    font-weight: 500;
}

#description{
    font-size: 10px;
    color: rgb(175, 172, 172);
}

.button1{
    background-color: #0089cf;
    color:white;
    text-decoration: none;
    border: none;
    padding:5px 10px;
    margin: 5px;
    text-align: center;
    border-radius: 12px;
    transition: all 0.5s;
    cursor: pointer;
}

.button1 span{
    cursor: pointer;
    display: inline-block;
    position: relative;
    transition: 0.5s;
}

.button1 span:after{
    content:'\00bb';
    position: absolute;
    opacity: 0;
    top: 0;
    right: -20px;
    transition: 0.5s;
}

.button1:hover span{
    padding-right: 15px;
}

.button1:hover span:after{
    opacity: 1;
    right: 0;
}

.button2{ 
    background-color: white;
    color: black;
    text-decoration: none;
    border: 1px solid #0089cf;
    padding:5px 10px;
    margin: 5px;
    text-align: center;
    border-radius: 12px;
    transition: all 0.5s;
    cursor: pointer; 
    transition-duration: 0.4s;
}

.button2:hover {
    background-color: #0089cf;
    color: white
}

#sign-in{
    font-size: 10px;
    color:rgb(175, 172, 172);
}

#sign-in2:link{
    color: #0089cf;
    font-size: 10px;
    color:rgb(175, 172, 172);
    text-decoration: none;
    cursor: pointer;
}

#sign-in2:visited{
    text-decoration: none;
    color:blueviolet;
}

#sign-in2:hover{
    text-decoration: underline;
}

#sign-in2:active{
    text-decoration: underline;
}

.bottom{ 
    color:black;
    font-size: 10px;
    display: inline;
}


.dot{
    height:5px;
    width:5px;
    background-color: #0089cf;
    border-radius: 50%;
    display: inline-block;
}

.right{
    width: 40%;
    display:grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    display:flex;
    justify-content: center;
    flex-wrap: wrap;
    flex-grow: 0;
}

.container {  
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    gap: 5px;
    grid-auto-flow: row;
    margin: 10px;
    background-color: rgb(243, 243, 243);
    border-radius: 15%;
}

#text{
    font-size: 10px;
}

.item1 {
    grid-area: 1 / 1 / 2 / 2;
    text-align: center;
    background-color: #0089cf;
    border-radius: 50%;
    height: 90px;
    width: 90px;
    color: white;
    line-height: 10px;
}

.item2 {
    grid-area: 1 / 2 / 2 / 3;
    text-align: center;
    border-radius: 0 50% 0 0;
    height: 90px;
    width: 90px;
    color: black;
    line-height: 10px;
    background-color: white;
}

.item3 {
    grid-area: 1 / 3 / 2 / 4;
    text-align: center;
    background-color: #0089cf;
    border-radius: 0 0 50% 0;
    height: 90px;
    width: 90px;
    color: white;
    line-height: 10px;
}

.item4 {
    grid-area: 2 / 1 / 3 / 2;
    text-align: center;
    background-color: #0089cf;
    border-radius: 0 0 0 50%;
    height: 90px;
    width: 90px;
    color: white;
    line-height: 10px;
}

.item5 { 
    grid-area: 2 / 2 / 3 / 3;
    text-align: center;
    border-radius: 50%;
    height: 90px;
    width: 90px;
    color: black;
    line-height: 10px;
    background-color: white;
}

.item6 { 
    grid-area: 2 / 3 / 3 / 4;
    text-align: center;
    background-color: #0089cf;
    border-radius: 50% 0 0 0;
    height: 90px;
    width: 90px;
    color: white;
    line-height: 10px;
}

.item7 {
    grid-area: 3 / 1 / 4 / 2; 
    text-align: center;
    background-color: #0089cf;
    border-radius: 0 50% 0 0;
    height: 90px;
    width: 90px;
    color: white;
    line-height: 10px;
}

.item8 { 
    grid-area: 3 / 2 / 4 / 3;
    text-align: center;
    border-radius: 0 0 50% 0;
    height: 90px;
    width: 90px;
    color: black;
    line-height: 10px;
    background-color: white;
}

.item9 { 
    grid-area: 3 / 3 / 4 / 4;
    text-align: center;
    background-color: #0089cf;
    border-radius: 50%;
    height: 90px;
    width: 90px;
    color: white;
    line-height: 10px;
}

.fa-solid{
    color: black;
}

.item1:hover{
    transition: all 0.5s;
    transition-duration: 0.4s;
    cursor: pointer
}


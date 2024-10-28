<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
.Sidebar {
    position: relative; /* Required for absolute positioning of hover box */
}

.Navigation {
    display: flex;
    flex-direction: column; /* Align links vertically */
}

.nav-link {
    text-decoration: none; /* Remove underline */
    color: black; /* Link color */
    padding: 10px; /* Space around links */
    transition: background-color 0.3s; /* Smooth transition for background color */
}

.nav-link:hover {
    background-color: lightgray; /* Background color on hover */
}

.hover-box {
    display: none; /* Hide the box by default */
    position: absolute; /* Positioning it absolutely */
    background-color: lightblue; /* Background color */
    padding: 10px; /* Some padding */
    border: 1px solid #ccc; /* Border */
    z-index: 1; /* Make sure it’s above other content */
}

/* Show the hover box next to the hovered link */
.nav-link:hover + .hover-box {
    display: block; /* Show the box on hover */
}

/* Positioning the hover box */
.nav-link:hover + .hover-box {
    left: 120%; /* Adjust as needed */
    top: 0; /* Align to the top of the link */
}

    </style>
</head>
<body>
    <div class="Sidebar">
        <div class="Navigation">
            <a href="#" class="nav-link" data-hover="Home Info"><b>HOME</b></a>
            <a href="#" class="nav-link" data-hover="School Objectives Info"><b>SCHOOL OBJECTIVES</b></a>
            <a href="#" class="nav-link" data-hover="School Department Info"><b>SCHOOL DEPARTMENT</b></a>
            <a href="#" class="nav-link" data-hover="Game Info"><b>GAME</b></a>
            <a href="#" class="nav-link" data-hover="About Us Info"><b>ABOUT US</b></a>
        </div>
        <div class="hover-box"></div>
    </div>
    <div class="bak1"></div>
    <div class="bak2"></div>
    <div class="bak3"></div>
    <div class="bak4"></div>
    <div class="bak5"></div>
</body>
</html>

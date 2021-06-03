# andrebestrada.github.io
Skip to content
Search or jump to…

Pull requests
Issues
Marketplace
Explore
 
@andrebestrada 
DataAnalyst77002
/
HTML-CSS-Homework
1
02
Code
Issues
Pull requests
Actions
Projects
Wiki
Security
Insights
HTML-CSS-Homework/index.html
@DataAnalyst77002
DataAnalyst77002 Update index.html
Latest commit a46ce82 on 19 Oct 2019
 History
 1 contributor
162 lines (150 sloc)  7.75 KB
  
<!DOCTYPE html>
<html lang="en">

<head>
<!--What needs to be loaded before getting into the code. -->
  <meta charset="UTF-8">
<!-- The title is here! -->
  <title>Latitude Analysis Dashboard</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- reset css -->
  <link rel="stylesheet" href="reset.css">
  <!-- Bring in our bootstrap stylesheet -->
  <link rel="stylesheet" 
  href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css">
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
     <!-- jQuery first, then Popper.js, then Bootstrap JS -->
     <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js" integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN" crossorigin="anonymous"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>
     <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>

    <!-- A black horizontal navbar that becomes vertical on small screens -->
    <nav class="navbar navbar-expand-sm navbar-blue">
        <a class="nav-link" href="https://dataanalyst77002.github.io/HTML-CSS-Homework/index.html"> <!-- button which links to index that appears only when clicked near the labels -->
            <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" 
            aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"> </span>
            </button>
        </a>
        <ul class="navbar-nav">
            <!-- Home button -->
            <li class="nav-item active">
                <a class="nav-link" href="https://dataanalyst77002.github.io/HTML-CSS-Homework/index.html">  
                Weather and Latitude</a>
            </li>
        </ul>

        <!-- right side of navbar -->
        <ul class="navbar-nav ml-auto">
            <li class="nav-item dropdown ml-auto">
                <a class="nav-link dropdown-toggle" data-toggle="dropdown" id="navbarDropdownMenuLink" href="#" role="button" 
                aria-haspopup="true" aria-expanded="false">Plot</a>
                <div class="dropdown-menu dropdown-menu-right" aria-labelledby="navbarDropdownMenuLink">
                    <a class="dropdown-item" href="https://dataanalyst77002.github.io/HTML-CSS-Homework/Temperature vs Latitude.html">Temperature</a>
                    <a class="dropdown-item" href="https://dataanalyst77002.github.io/HTML-CSS-Homework/Humidity vs Latitude.html">Humidity</a>
                    <a class="dropdown-item" href="https://dataanalyst77002.github.io/HTML-CSS-Homework/Cloudiness vs Latitude.html">Cloudiness</a>
                    <a class="dropdown-item" href="https://dataanalyst77002.github.io/HTML-CSS-Homework/Windiness vs Latitude.html">Wind Speed </a>
                </div>
            </li> 
            <li class="nav-item">
                <a class="nav-link" href="https://dataanalyst77002.github.io/HTML-CSS-Homework/Comparison_Page.html">Comparison
                </a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="https://dataanalyst77002.github.io/HTML-CSS-Homework/Data_Page.html">Data</a>
            </li>
        </ul>
    </nav>

    <!-- Main Body: Twitter bootstrap -->
      <div style="background-color:goldenrod;">
        <div class="row">
            <div class="col-md-12">
                </br>
                </br> <!-- line break to push header down -->
            </div>
        </div>
      </div> <!-- background color -->
        <!-- Header -->
    <div class = 'container-fluid'>
        <div class="row align-items-center">
            <div class = 'col-md-4'></div>
            <div class="col-lg-4">
                <h1 class="intro">Project Summary</h1>
            </div>
            <div class = 'col-md-4'> </br> </br> </div>
        </div>
        <!-- line breaks to push header down -->
        <div class="row">
            <div class="col-md-12">
                </br> 
                </br>
            </div>
        </div>

        <!-- main content -->
        <div class="row align-items-center">
            <!-- summary paragraph -->
            <div class="col-lg-6">
                <p>In this project, I sought to analyze weather patterns based on 
                distance to the equator. I utilized Python script to visualize the weather of 500+ cities 
                across the world of varying distance from the equator.  To accomplish this, I utilizing
                a simple Python library, the OpenWeatherMap API to create representative
                models of weather across world cities.
                </br>
                </br>
                I first assembled a dataset of more than 500 cities using the 
                citipy python library and python to randomly generate coordinates to get the
                nearest city. Then I use this list of cities to get the weather using the OpenWeatherMap API.
                Using MatPlotLib, I used each city's maximum temperature, humidity, cloudiness, or wind speed and plotted
                the data with the latitude on the appropriate graphs. 
                </br>
                </p>
                
            </div>
            
        </div>
    </div>

    <!-- Visualizations -->
        <!-- Header -->
    <div id = "bottom_visual" class="container"> 
        <div class="row">
            <div class="col-md-12">
                </br> <!-- line break to push header down -->
            </div>
        </div>
        <hr> <!-- horizontal line -->

        <!-- Header content for visualization section -->
        <div class="row align-items-center">
            <div class = 'col-md-4'></br></br></br></div>
            <div class="col-lg-4">
                <h3 id="bot_header">Graphic Visualizations</h3>
            </div>
            <div class = 'col-md-4'></br></br></br></div>
        </div>

        <div class="row align-items-center">
            <div class="col-lg-3">
                <a href="Temperature vs Latitude.html">
                    <img class="mx-auto d-block img-fluid" src="Resources\Temperatures-n-World_Cities.png"
                    alt = "Maximum Temperature vs. Latitude" height="225" width="300">
                </a>
            </div>
            <div class="col-lg-3">
                <a href="Humidity vs Latitude.html">
                    <img class="mx-auto d-block img-fluid" src="Resources\Humidity-n-World_Cities.png"
                    alt = "Humidity vs. Latitude" height="225" width="300">
                </a>
            </div>
            <div class="col-lg-3">
                <a href="Cloudiness vs Latitude.html">
                    <img class="mx-auto d-block img-fluid" src="Resources\Cloudiness-n-World_Cities.png"
                    alt = "Cloudiness vs. Latitude" height="225" width="300">
                </a>
            </div>
            <div class="col-lg-3">
                <a href="Windiness vs Latitude.html">
                    <class="mx-auto d-block img-fluid" src="Resources\Wind_Speed-n-World_Cities.png"
                    alt = "Windspeed vs. Latitude" height="225" width="300">
                </a>
            </div>
        </div>
    
        <hr>
    </div>
</body>
</html>
© 2021 GitHub, Inc.
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
Loading complete

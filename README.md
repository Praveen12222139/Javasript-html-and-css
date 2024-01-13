# Javasript-html-and-css
Weather app using Javascript , css and html
<!doctype html>
<html lang="en">
    <link rel="icon" href="icon.png">
  <head>
    <style>
      #cityName{
        color: red;
      }
      h2{
        color: blueviolet;
        
      }
     
    </style>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Weather App</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-rbsA2VBKQhggwzxH7pPCaAqO46MgnOM80zW1RWuH61DGLwZJEdK2Kadq2F9CUG65" crossorigin="anonymous">
  </head>
  <body>
    <nav class="navbar navbar-expand-lg bg-light">
        <div class="container-fluid">
          <a class="navbar-brand" href="#">Weather App</a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0">
              <li class="nav-item">
                <a class="nav-link active" aria-current="page" href="#">Home</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">About this App</a>
              </li>
              <li class="nav-item dropdown">
                <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                
                </a>
                <ul class="dropdown-menu">
                  <li><a class="dropdown-item" href="#"> Delhi</a></li>
                  <li><a class="dropdown-item" href="#">Akhnoor</a></li>
                  <li><hr class="dropdown-divider"></li>
                  <li><a class="dropdown-item" href="#">Fatehpur</a></li>
                </ul>
              </li>
              <li class="nav-item">
                <a class="nav-link disabled">Usage Guide</a>
              </li>
            </ul>
            <form class="d-flex" role="search">
              <input id="city" class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
              <button class="btn btn-outline-success" type="submit" id="submit">Search</button>
            </form>
          </div>
        </div>
      </nav>

      <div container="">
        <h1 class="my-4 text-center">Weather for  <span id="cityName"></span></h1>
        <main>
            <div class="row row-cols-1 row-cols-md-3 mb-3 text-center">
              <div class="col">
                <div class="card mb-4 rounded-3 shadow-sm">
                  <div class="card-header py-3">
                    <h4 class="my-0 fw-normal">Temperatures</h4>
                  </div>
                  <div class="card-body">
                    <h1 class="card-title pricing-card-title"><span id="temp2"></span><small class="text-muted fw-light"><span>&#8451;</span></small></h1>
                    <ul class="list-unstyled mt-3 mb-4">
                      <li>Temperature is <span id="temp"></span></li>
                      <li>Min Temperature is <span id="min_temp"></span></li>
                      <li>Maximum Temperture  is <span id="max_temp"></span></li>
                      
                    </ul>
                    <button type="button" class="w-100 btn btn-lg btn-outline-primary">Click for more info</button>
                  </div>
                </div>
              </div>
              <div class="col">
                <div class="card mb-4 rounded-3 shadow-sm">
                  <div class="card-header py-3">
                    <h4 class="my-0 fw-normal">Humidity Info</h4>
                  </div>
                  <div class="card-body">
                    <h1 class="card-title pricing-card-title"><span id="humidity2"></span><small class="text-muted fw-light"> %</small></h1>
                    <ul class="list-unstyled mt-3 mb-4">
                      <li>Cloud PCT is <span id="cloud_pct"></span></li>
                      <li>Humidity is <span id="humidity"></span></li>
                      <li>Feels like is <span id="feels_like"></span></li>
                    
                    </ul>
                    <button type="button" class="w-100 btn btn-lg btn-primary">Click for more info</button>
                  </div>
                </div>
              </div>
              <div class="col">
                <div class="card mb-4 rounded-3 shadow-sm border-primary">
                  <div class="card-header py-3 text-bg-primary border-primary">
                    <h4 class="my-0 fw-normal">Wind And Sun Info</h4>
                  </div>
                  <div class="card-body">
                    <h1 class="card-title pricing-card-title"><span id="wind_speed2"></span><small class="text-muted fw-light"> Km/hr</small></h1>
                    <ul class="list-unstyled mt-3 mb-4">
                        <li>Wind Speed is <span id="wind_speed"></span></li>
                      <li>Wind Degree is <span id="wind_degrees"></span></li>
                      <li>Sunset Time <span id="sunset"></span></li>
                      <li>Sunrise Time <span id="sunrise"></span></li>
                    </ul>
                    <button type="button" class="w-100 btn btn-lg btn-primary">Click for more info</button>
                  </div>
                </div>
              </div>
            </div>
        
            <h2 class="display-6 text-center mb-4">Weather of other common places</h2>
        
            <div class="table-responsive">
              <table class="table text-center">
                <thead>
                  <tr>
                    <th style="width: 34%;"></th>
                    <th style="width: 22%;"> cloud_pct </th>
                    <th style="width: 22%;"> Feels_like</th>
                    <th style="width: 22%;"> Humidity</th>
                    <th style="width: 22%;"> Max_temp</th>
                    <th style="width: 22%;"> Min_temp</th>
                     <th style="width: 22%;"> Sunrise</th>
                    <th style="width: 22%;"> Sunset</th>
                    <th style="width: 22%;"> Temp</th>
                    <th style="width: 22%;"> Wind_degrees</th>
                    <th style="width: 22%;"> Wind_speed</th>
                  </tr>
                </thead>
                <tbody>
                  <tr>
                    <th scope="row" class="text-start">London</th>
                    <td>1</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                  </tr>
                  <tr>
                    <th scope="row" class="text-start">Paris</th>
                    <td>1</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                  </tr>
                </tbody>
        
                <tbody>
                  <tr>
                    <th scope="row" class="text-start">Kolkata</th>
                    <td>1</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                  </tr>
                  <tr>
                    <th scope="row" class="text-start">Shimla</th>
                    <td>1</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                  </tr>
                  <tr>
                    <th scope="row" class="text-start">Vaishno Devi</th>
                    <td>1</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                  </tr>
                  <tr>
                    <th scope="row" class="text-start">Suratgarh</th>
                    <td>1</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                    <td>2</td>
                  </tr>
                </tbody>
              </table>
            </div>
          </main>
      </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-kenU1KFdBIe4zVF0s0G1M5b4hcpxyD9F7jL+jjXkk+Q2h455rYXK/7HAuoJl+0I4" crossorigin="anonymous"></script>
 <script src="script.js"></script>
</body>
</html>

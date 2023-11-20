WEATHER.HTML:
-----------------------------------

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <!-- Nicholas J. Corkigian, 123456789 -->
    <title>Weather</title>
    <link href="weather.css" rel="stylesheet" type="text/css">
    <style>
      main
      {
        display: grid;
        grid-gap: 20px;
        grid-template-columns: auto 250px;
        margin: 10px 100px;
      }
      
      h1
      {
        background-color: #fdb924;
        margin: 10px 0px;
        padding-left: 10px;
      }
      
      section p 
      {
        margin-bottom: 10px;
      }
      
      aside
      {
        background-image: url(images/background/clouds.jpg);
      }
      
      aside p
      {
        margin: 0px 10px;
      }
      
      aside ol 
      {
        padding-left: 30px;
      }
      
      aside li 
      {
        list-style-type: lower-roman;
      }
      
      article
      {
        grid-column: 1 / 3;
      }
      
      article div
      {
        display: flex;
        flex-flow: row wrap;
      }
      
      article figure
      {
        border: 2px solid #808080;
        margin: 20px;
      }
      
      article figure figcaption
      {
        text-align: center;
      }
      
      section div
      {
        display: flex;
        flex-flow: row nowrap;
      }
      
      section div figure
      {
        border: 1px solid #808080;
        flex: 1 1 100px;
        padding: 5px;
      }
      
      section span
      {
        font-size: larger;
        font-weight: bold;         
      }
      
      section h5
      {
        margin-top: 10px;
      }
      
      section img
      {
        display: block;
        height: 100px;
        width: 100%;
      }
    </style>
  </head>
  
  <body>
    <nav>
      <ul>
        <li><a href="#">Today's Weather</a></li>
        <li><a href="#">Clouds</a></li>
        <li><a href="#">Wild Weather</a></li>
        <li><a href="#">Contact Us</a></li>
      </ul>
    </nav>
    
    <header>
      <img src="images/logos/weathernow.png" alt="Weather">
      
      <div id="social">
        <a href="https://www.facebook.com"><img src="images/socialmedia/facebook32.png" alt="Facebook"></a>
        <a href="https://www.twitter.com"><img src="images/socialmedia/twitter32.png" alt="Twitter"></a>
        <a href="mailto:weather@example.com"><img src="images/socialmedia/emailat32.png" alt="Email"></a>
      </div>
    </header>
    
    <main>
      <section>
        <h1>Forecast</h1>

        <div>
          <figure>
            <h4>Today</h4>
            <img src="images/weathericons/cloud.png" alt="Cloudy">
            <span>15&deg;C</span>/8&deg;C
            <h5>Cloudy</h5>
          </figure>
          
          <figure>
            <h4>Tomorrow</h4>
            <img src="images/weathericons/suncloudstorm.png" alt="Cloudy with Thunderstorm in the morning">
            <span>18&deg;C</span>/4&deg;C
            <h5>Cloudy with Thunderstorm in the morning</h5>
          </figure>
          
          <figure>
            <h4>Friday</h4>
            <img src="images/weathericons/rain.png" alt="Rainy all day">
            <span>12&deg;C</span>/6&deg;C
            <h5>Rainy all day</h5>
          </figure>
          
          <figure>
            <h4>Saturday</h4>
            <img src="images/weathericons/suncloud.png" alt="Sun with clouds">
            <span>21&deg;C</span>/10&deg;C
            <h5>Sun with clouds</h5>
          </figure>
          
          <figure>
            <h4>Sunday</h4>
            <img src="images/weathericons/suncloud.png" alt="Sun with clouds">
            <span>24&deg;C</span>/12&deg;C
            <h5>Sun with clouds</h5>
          </figure>
          
        </div>
        
        <h1>Forecasting</h1>
        <p>
          Weather forecasting is the application of science and technology 
          to predict the state of the atmosphere for a future time and a 
          given location. Human beings have attempted to predict the weather 
          informally for millennia, and formally since at least the 
          nineteenth century.[27] Weather forecasts are made by collecting 
          quantitative data about the current state of the atmosphere and 
          using scientific understanding of atmospheric processes to project 
          how the atmosphere will evolve.
        </p>
        
        <p>
          Once an all-human endeavor based mainly upon changes in barometric 
          pressure, current weather conditions, and sky condition, forecast 
          models are now used to determine future conditions. On the other 
          hand, human input is still required to pick the best possible 
          forecast model to base the forecast upon, which involve many 
          disciplines such as pattern recognition skills, teleconnections, 
          knowledge of model performance, and knowledge of model biases.
        </p>
      </section>

      <aside>
        <h1>Clouds</h1>
        
        <p>
          In meteorology, a cloud is an aerosol consisting of a visible mass 
          of minute liquid droplets, frozen crystals, or other particles 
          suspended in the atmosphere of a planetary body or similar space. 
          Water or various other chemicals may compose the droplets and 
          crystals. On Earth, clouds are formed as a result of saturation of 
          the air when it is cooled to its dew point, or when it gains 
          sufficient moisture (usually in the form of water vapor) from an 
          adjacent source to raise the dew point to the ambient temperature.
        </p>

        <h1>Cloud Types</h1>
        
        <ol>
          <li>Stratiform</li>
          <li>Cirriform</li>
          <li>Stratocumuliform</li>
          <li>Cumuliform</li>
          <li>Cumulonimbiform</li>
        </ol>
      </aside>
      
      <article>
        <h1>Wild Weather</h1>
        
        <div id="gallery">
          <figure>
            <img src="images/weatherpics/weather1_tn.jpg" alt="Dust Storm">
            <figcaption>Dust Storm</figcaption>
          </figure>
          
          <figure>
            <img src="images/weatherpics/weather2_tn.jpg" alt="Tornado">
            <figcaption>Tornado</figcaption>
          </figure>
          
          <figure>
            <img src="images/weatherpics/weather3_tn.jpg" alt="Rain Storm">
            <figcaption>Rain Storm</figcaption>
          </figure>
          
          <figure>
            <img src="images/weatherpics/weather4_tn.jpg" alt="Lightning">
            <figcaption>Lightning</figcaption>
          </figure>
          
          <figure>
            <img src="images/weatherpics/weather5_tn.jpg" alt="Hurricane">
            <figcaption>Hurricane</figcaption>
          </figure>
          
          <figure>
            <img src="images/weatherpics/weather6_tn.jpg" alt="Rain Storm">
            <figcaption>Rain Storm</figcaption>
          </figure>
          
          <figure>
            <img src="images/weatherpics/weather7_tn.jpg" alt="Tornadoes">
            <figcaption>Tornadoes</figcaption>
          </figure>
          
        </div>
      </article>
    </main>
    
    <footer>
      <img src="images/logos/weathernow_horiz.png" alt="weathernow">
      
      <div>
        <h4>Contact Us</h4>
        Email<br>
        Phone
        <br><br>
        <h4>Apps</h4>
        WeatherNow iOS<br>
        WeatherNow Android
      </div>
      
      <div>
        <h4>Support</h4>
        FAQs<br>
        Privacy Policy<br>
        Terms of Use
      </div>
      
      <div>
        <h4>Social</h4>
        <a href="https://www.facebook.com"><img src="images/socialmedia/facebook32.png" alt="Facebook"></a>Facebook<br>
        <a href="https://www.twitter.com"><img src="images/socialmedia/twitter32.png" alt="Twitter"></a>Twitter<br>
        <a href="mailto:weather@example.com"><img src="images/socialmedia/emailat32.png" alt="Email"></a>weather@example.com
      </div>
      
      
    </footer>
  </body>
</html>




---------------
CSS:
@charset "utf-8";

/* Nicholas J. Corkigian, 123456789 */

*
{
  box-sizing: border-box;
  margin: 0px;
  padding: 0px;
  list-style-type: none;
  text-decoration: none;
}

body
{
  font-family: Arial, Helvetica, Verdans, sans-serif;
  min-width: 620px;
}

nav
{
  background-color: black;
  padding: 0px 20px;
  position: sticky;
  top: 0px;
}

nav::after
{
  content: "";
  clear: both;
  display: table;
}

nav li 
{
  float: left;
  padding: 10px 10px;
  margin: 0px 1em;
}


nav li:hover
{
  background-color: #808080;
}

nav a 
{
  color: #fdb924;
}

nav a:hover
{
  text-decoration: underline;
}

header
{
  display: grid;
  grid-template-columns: 1fr auto;
}

header > img
{
  justify-self: center;
}

header div#social
{
  align-self: center;
}

footer
{
  background-color: #fdb924;
  display: grid;
  grid-gap: 60px;
  grid-template-columns: auto 1fr 1fr 1fr;
  padding: 20px 0px 0px 20px;
}

h4
{
  border-bottom: 1px solid black;
}

footer div img
{
  margin-right: 2px;
  vertical-align: middle;
}



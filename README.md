<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <!-- Nicholas J. Corkigian, 123456789 -->
    <title>Soccer Camp</title>
    <style>
      *
      {
        box-sizing: border-box;
        margin: 0;
        padding: 0;        
      }
      
      body
      {
        margin: 0px auto 2em;
        width: 90%;
      }
      
      main
      {
        display: grid;
        grid-gap: 20px;
        grid-template-columns: 2fr 1fr;
      }
      
      header h1
      {
        color: #D3D3D3;
        font-family: 'Courier New', sans-serif;
        font-size: 2em;
        margin: 10px;
        text-align: center;
      }
      
      footer
      {
        border-top: 1px solid black;
        font-family: Calibri, sans-serif;
        font-size: 0.75em;
        margin-top: 2em;
        text-align: center;
      }
      
      table
      {
        border: 1px solid black;
        border-collapse: collapse;
        font-family: Arial, sans-serif;
        height: 100%;
        width: 100%;
      }
      
      table caption
      {
        caption-side: bottom;
        font-family: 'Times New Roman', serif;
      }
      
      table th, table td
      {
        border: 1px solid black;
        font-weight: normal;
        padding: 1em 0px 1em 5px;
        text-align: left;
      }
      
      table thead
      {
        background-color: black;
        color: white;
        font-family: 'Times New Roman', serif;
        padding: 1em 0px;
      }
      
      table thead th
      {
        font-weight: bold;
        text-align: center;
      }
      
      table col#firstCol
      {
        background-color: #D3D3D3;
        width: 15%;
      }
      
      table col.restDays
      {
        width: 12%;
      }
      
      aside
      {
        font-family: Arial, sans-serif;
      }
      
      form
      {
        border: 1px solid black;
        padding: 10px;
        width: 100%;
      }
      
      form h2
      {
        margin-top: 0px;
      }
      
      form fieldset
      {
        border: 1px solid black;
        margin: 5px 0px;
        padding: 10px;
      }
      
      form legend
      {
        padding: 0px 25px;
      }
      
      form fieldset#ident label
      {
        display: inline-block;
        margin-right: 10px;
        text-align: right;
        width: 100px;
      }
      
      form fieldset#ident label.radio
      {
        display: inline;
      }
      
      form textarea
      {
        height: 6em;
        width: 90%;
      }
      
      form #buttons input
      {
        background-color: white;
        border: 0px solid black;
        margin-right: 10px;
        text-decoration: underline;
      }
      
      @media only screen and (max-width: 600px)
      {
        main
        {
          display: block;
        }
      }
    </style>
  </head>
  
  <body>
    <header>
      <h1>Soccer Camp Registration</h1>
    </header>
    
    <main>
      <aside>
        <table>
          <caption>July Weekly Schedule</caption>
          
          <colgroup>
            <col id="firstCol">
            <col class="restDays" span="7">
          </colgroup>
          
          <thead>
            <tr>
              <th></th>
              <th>Sun</th>
              <th>Mon</th>
              <th>Tue</th>
              <th>Wed</th>
              <th>Thur</th>
              <th>Fri</th>
              <th>Sat</th>            
            </tr>
          </thead>
          
          <tbody>
            <tr>
              <th>9:00am - 10:30am</th>
              <td>Free Time</td>
              <td rowspan="3">Technical Skills</td>
              <td colspan="4">Training Session</td>
              <td>Free Time</td>
            </tr>
            
            <tr>
              <th>10:30am - 12:00pm</th>
              <td rowspan="3">Round Robin Games</td>
              <td rowspan="2" colspan="3">Dribbling</td>
              <td rowspan="2">Game Analysis</td>
              <td>Agility</td>
            </tr>
            
            <tr>
              <th>1:00pm - 2:30pm</th>
              <td>Strength Training</td>
            </tr>
            
            <tr>
              <th>2:30pm - 5:00pm</th>
              <td colspan="3">Nutrition</td>
              <td>Passing and Receiving</td>
              <td rowspan="2" colspan="2">Camper's Choice</td>
            </tr>
            
            <tr>
              <th>6:00pm - 8:00pm</th>
              <td colspan="5">Night Games</td>
            </tr>
          </tbody>
        </table>
      </aside>
      
      <aside>
        <form action="https://csunix.mohawkcollege.ca/tooltime/showit.pl" method="post">
          <h2>Request Camp Information</h2>
          <input type="hidden" name="formname" value="Nicholas Corkigian">
          
          <fieldset>
            <legend>Camper Location</legend>
            
            <label for="location">Province</label>
            <select name="location" id="location">
              <option value="BC">British Columbia</option>
              <option value="AB">Alberta</option>
              <option value="ON" selected>Ontario</option>
              <option value="QC">Quebec</option>
              <option value="YT">Yukon</option>
            </select>
          </fieldset>
          
          <fieldset id="ident">
            <legend>Camper Identification</legend>
            
            <div class="formRow">
              <label for="firstName">First Name</label>
              <input id="firstName" name="firstName">
            </div>
            
            <div class="formRow">
              <label for="lastName">Last Name</label>
              <input id="lastName" name="lastName">
            </div>

            <div class="formRow">
              <label>Gender</label>
              <input type="radio" name="gender" id="male" value="male" checked>
              <label class="radio" for="male">Male</label>
              <input type="radio" name="gender" id="female" value="female">
              <label class="radio" for="female">Female</label>
            </div>

            <div class="formRow">
              <label for="email">Email</label>
              <input id="email" name="email" type="email" placeholder="name@example.com">
            </div>

            <div class="formRow">
              <label for="age">Camper Age</label>
              <select name="age" id="age">
                <option value="8">8-9</option>
                <option value="10">10-12</option>
                <option value="13">13-15</option>
                <option value="16">16-19</option>
              </select>
            </div>
          </fieldset>
          
          <fieldset>
            <legend>Please send me information about</legend>

            <div class="formRow">
              <input type="checkbox" name="info" value="dates" id="dates">
              <label for="dates">Camp Dates</label>
            </div>
            
            <div class="formRow">
              <input type="checkbox" name="info" value="fees" id="fees">
              <label for="fees">Camp fees</label>
            </div>
            
            <div class="formRow">
              <input type="checkbox" name="info" value="transport" id="transport" checked>
              <label for="transport">Transportation</label>
            </div>

          </fieldset>
          
          <fieldset>
            <legend>Question?</legend>
            
            <textarea name="questions">Please enter questions or comments here</textarea>
          </fieldset>
          
          <div id="buttons">
            <input type="Submit" value="Request Info">
            <input type="Reset" value="Clear Form">
          </div>
        </form>
      </aside>
    </main>
    
    <footer>
      Mohawk College of Applied Arts and Technology
    </footer>
  </body>
</html>

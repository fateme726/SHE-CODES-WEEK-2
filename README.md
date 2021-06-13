<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>weathering with you</title>
    <style>
      h1 {
        color: blue;
        text-align: center;
        font-size: 36px;
        font-weight: bold;
      }

      h2 {
        text-align: center;
        font-size: 32px;
      }
      h4 {
        text-align: center;
        font-size: 32px;
        color: blue;
      }

      ul {
        list-style: none;
        text-align: center;
        padding: 0;
      }

      li {
        list-style-type: none;
        padding: 10px 0;
        display: block;
        margin: 0 auto;
        max-width: 400px;
      }
      li:hover {
        list-style-type: none;
        background-color: peachpuff;
        padding: 10px o;
        display: block;
        margin: auto;
        transition: all 200ms ease-in-out;
        border-radius: 10px;
      }
      button {
        display: block;
        margin: 20px auto;
        padding: 20px 20px;
        border-radius: 30px;
        color: white;
        font-size: 16px;
        background-color: blue;
        border: 1px solid blue;
        box-shadow: rgb(37 39 89 / 8%) 0px 8px 8px 0;
      }
      button:hover {
        display: block;
        margin: 20px auto;
        padding: 20px 20px;
        border-radius: 30px;
        color: blue;
        font-size: 16px;
        background-color: white;
        border: 1px solid blue;
        transition: all 100ms ease-in-out;
        box-shadow: rgb(37 39 89 / 8%) 0px 8px 8px 0;
      }
      p {
        color: grey;
        text-align: center;
        font-size: 18px;
      }
    </style>
  </head>

  <body>
    <h1>
      🌤
      </h1>
      <h4>
 Currently 21° in Tokyo
      </h4>
     
     

      

    <h2>13°/ <strong>23°</strong></h2>
    <ul>
      <li>
        <h3>🌧Tomorrow</h3>
        <p>
          10°/
          <strong>22°</strong>
        </p>
      </li>
      <li>
        <h3>🌥 Saturday</h3>
        <p>
          15°/
          <strong>17°</strong>
        </p>
      </li>
      <li>
        <h3>☀️ Sunday</h3>
        <p>
          25°/
          <strong>28°</strong>
        </p>
      </li>
    </ul>

    <button>Change city</button>
    <p>Coded by Fatemeh Yousefi</p>
    <script>
      function changeCity(){
        let city = prompt ( "what city do you live in?");
        let temprature = prompt ( "what is the temprature?");
        let h4 = document.querySelector("h4");  
        let h1 = document.querySelector("h1");
        h4.innerHTML ="currently " + temprature + " in " + city;
        if ( temprature <0) {
          h1.innerHTML = "😰";
    } 
    else {
      h1.innerHTML = "😍"
    }
    } 
     let cityButton = document.querySelector("button");
     cityButton.addEventListener("click", changeCity);
    
    </script>
  </body>
</html>

# SHE-CODES-WEEK-2
SHE CODES WEEK 2 CHALLENGES
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>shecodesweek2</title>

    <style>
      h1 {
        text-align: center;
      }
     
      li{
        text-align: center;
        list-style-type: none;
        padding: 4px;
      }
      button{
        display: block;
        margin: 0 auto;
        margin-top: 12px;
      }
    </style>
  </head>

  <body>
    <h1>👩🏻‍💻shecodes</h1>
    <ui>
      <li class="advanced">SheCodes+</li>
      <li class="free">SheCodes Express</li>
      <li class="free">SheCodes Story</li>
    </ui>
    <button>
      contact us
    </button>
    <script>
     function applyNow (){
     let name = prompt ("what is your name?");
     let age = prompt ("how old are you?");
     let h1 = document.querySelector("h1");
     if (age >= 18) {
     h1.innerHTML = "Hi, " + name + "!" + ", welcome to SheCodes";
     } else {
       h1.innerHTML = "sorry, " + name   + "!" +  ", You cannot join SheCodes";
     }
     }
          let contactButton = document.querySelector("button");
          contactButton .addEventListener("click", applyNow);

    </script>
  </body>
</html>

<!DOCTYPE html>
<html>
<head>
    <title>login UI</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" integrity="sha384-wvfXpqpZZVQGK6TAh5PVlGOfQNHSoD2xbE+QkPxCAFlNEevoEH3Sl0sibVcOQVnN" crossorigin="anonymous">
        <link rel="stylesheet" type="text/css"
              href="style.css">
</head>
<body>
<style>
    body {
      font-family: "Open Sans", sans-serif;
      height: 100vh;
      
    position:fixed;
    width:99%;
    height:99%;
    background:#222;
    margin:0;
    border:10px solid red;
    border-radius:10px;
    animation-iteration-count:infinite;
    animation-duration:2s;
    animation-name:ba;
}

@keyframes ba{
    20%{
        border:2px solid magenta;
    }
    40%{
        border:6px solid orange;
    }
    60%{
        border:10px solid green;
    }
    80%{
        border:14px solid purple;
    }
    95%{
        border:19px solid lime;
    }
}
   
    
    * {
      box-sizing: border-box;
    }
    
    .wrapper {
      display: flex;
      align-items: center;
      flex-direction: column;
      justify-content: center;
      width: 100%;
      min-height: 100%;
      padding: 20px;
      background:transparent;
    }
    
    .login {
      border-radius: 2px 2px 5px 5px;
      padding: 10px 20px 20px 20px;
      width: 90%;
      max-width: 320px;
      background: #ececec;
      position: relative;
      padding-bottom: 80px;
      box-shadow: 0px 1px 5px rgba(0, 0, 0, 0.3);
    }
    
    .login.loading button {
      max-height: 100%;
      padding-top: 50px;
    }
    
    .login.loading button .spinner {
      opacity: 1;
      top: 40%;
    }
    
    .login.ok button {
      background-color: #8bc34a;
    }
    
    .login.ok button .spinner {
      border-radius: 0;
      border-top-color: transparent;
      border-right-color: transparent;
      height: 20px;
      animation: none;
      transform: rotateZ(-45deg);
    }
    
    .login input {
      display: block;
      padding: 15px 10px;
      margin-bottom: 10px;
      width: 100%;
      box-shadow:inset -10px -10px 15px rgba(255,255,255,0.55),
              inset 10px 10px 15px rgba(70,70,70,0.12);;
      border: 1px solid #ddd;
      transition: border-width 0.2s ease;
      border-radius: 2px;
      color: #ccc;
    }
    
    .login input+i.fa {
      color: #fff;
      font-size: 1em;
      position: absolute;
      margin-top: -47px;
      opacity: 0;
      left: 0;
      transition: all 0.1s ease-in;
    }
    
    .login input:focus {
      outline: none;
      color: #444;
      border-color: #2196F3;
      border-left-width: 35px;
    }
    
    
    .login a {
      font-size: 0.8em;
      color: #2196F3;
      text-decoration: none;
    }
    
    .login .title {
      color: #444;
      font-size: 1.2em;
      font-weight: bold;
      margin: 10px 0 30px 0;
      border-bottom: 1px solid #eee;
      padding-bottom: 20px;
    }
    
    .login button {
      width: 100%;
      height: 100%;
      padding: 10px 10px;
      background: #2196F3;
      color: #fff;
      display: block;
      border: none;
      margin-top: 20px;
      position: absolute;
      left: 0;
      bottom: 0;
      max-height: 60px;
      border: 0px solid rgba(0, 0, 0, 0.1);
      border-radius: 0 0 2px 2px;
      transform: rotateZ(0deg);
      transition: all 0.1s ease-out;
      border-bottom-width: 7px;
    }
    .logo
{
  position:relative;
  color: red;
  font-size: 2em;
  text-shadow: 0 0 1000px #0f0,
              0 0 100px #0f0,
              0 0 150px #0f0,
              0 0 200px #0f0,
              0 0 250px #0f0;
  animation: animate 7s linear infinite;            
}
@keyframes animate
{
  0%
  {
     filter: hue-rotate(0deg);
  }   
  100%
  {
     filter: hue-rotate(720deg);
  }   
}  
    
        

    
</style>
  <div class="wrapper">
    <form class="login">
      <p class="title">Log in</p>
       <div class="box">
      <i class="fa fa-user logo"
         aria-hidden="true"></i>
         
      <input type="text" placeholder="Username" autofocus/></div>
      <i class="fa fa-key logo"></i>
      <input type="password" placeholder="Password" />
      
      <a href="#">Forgot your password?</a>
      <button>
      Log in
    </button>
    </form>
    </p>
  </div>

  <style>
    
  </style>

</body>

</html>

# formylove.github.io
<!DOCTYPE html>
<html>
<head>
  <title>Login Page</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="container">
    <h2>Login</h2>
    <form id="loginForm">
      <div class="form-group">
        <label for="username">Username:</label>
        <input type="text" id="username" placeholder="Enter your username" required>
      </div>
      <div class="form-group">
        <label for="password">Password:</label>
        <input type="password" id="password" placeholder="Enter your password" required>
      </div>
      <button type="submit" class="btn">Login</button>
    </form>
  </div>

  <script>
    document.getElementById("loginForm").addEventListener("submit", function(event) {
      event.preventDefault();
      var username = document.getElementById("username").value;
      var password = document.getElementById("password").value;
      
      // Perform login validation here
      if (username === "admin" && password === "password")  {
        window.location.href = "body.html" ;
      } else {
        alert("Oh mali wag kana pumasok germs ka gawa ka account teh.");
      }
    });
  </script>
</body>
</html>

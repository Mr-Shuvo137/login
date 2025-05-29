<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Login – GRS Effort</title>
  <style>
    body {
      background: #f4f8fb;
      font-family: Arial, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }
    .login-container {
      background: white;
      padding: 40px;
      border-radius: 12px;
      box-shadow: 0 8px 16px rgba(0,0,0,0.2);
      text-align: center;
      width: 300px;
    }
    .login-container h2 {
      margin-bottom: 20px;
    }
    .login-container input {
      width: 100%;
      padding: 10px;
      margin-bottom: 15px;
      border: 1px solid #ccc;
      border-radius: 6px;
    }
    .login-container button {
      width: 100%;
      padding: 10px;
      background: #007bff;
      color: white;
      border: none;
      border-radius: 6px;
      cursor: pointer;
    }
    .login-container button:hover {
      background: #0056b3;
    }
    .forgot {
      display: block;
      margin-top: 10px;
      font-size: 12px;
      color: #007bff;
      text-decoration: none;
    }
  </style>
</head>
<body>
  <div class="login-container">
    <h2>Welcome to GRS Effort</h2>
    <form onsubmit="login(event)">
      <input type="text" id="username" placeholder="Your Username" required>
      <input type="password" id="password" placeholder="Enter Password" required>
      <button type="submit">Login</button>
      <a href="#" class="forgot">Forgot Password?</a>
    </form>
  </div>

  <script>
    function login(e) {
      e.preventDefault();
      const username = document.getElementById('username').value;
      const password = document.getElementById('password').value;
      if (username === 'shuvo' && password === '1234') {
        alert('Login Successful');
        // Redirect or load dashboard
      } else {
        alert('Invalid credentials');
      }
    }
  </script>
</body>
</html>



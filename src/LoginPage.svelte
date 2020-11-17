<script>
</script>

<style>
	main {
		background: #444;
		width: 100%;
		height: 100vh;
		color: #FF6347;
	}

	header {
		width: 300px;
		padding: 250px;
  	padding-top:75px;
	}
	
	.bottom {
		padding-top:200px;
	}
	
	.center {
		text-align: center; 
	}
	
	#welcome {
		font-size:8rem;
		text-align: center;
	}
	
	#welcomesub {
		text-align: center;
		font-size: 1.5rem;
	}
</style>

<form action="action_page.php" method="post">
  <div class="center">
    <label for="uname"><b>Username</b></label>
    <input type="text" placeholder="Enter Username" name="uname" required>

    <label for="psw"><b>Password</b></label>
    <input type="password" placeholder="Enter Password" name="psw" required>
	</div>
	<div class = "center">
    <button type="submit">Login</button>
    <label>
      <input type="checkbox" checked="checked" name="remember"> Remember me
    </label>
	</div>

  <div class="center bottom">
    <span class="psw">Forgot <a href="#">password?</a></span>
  </div>
</form>
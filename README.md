<head>

<link href="http://fonts.googleapis.com/css?family=Oswald" rel="stylesheet" type="text/css" />
<link href='http://fonts.googleapis.com/css?family=Arvo' rel='stylesheet' type='text/css'>
<link href="../css/style1.css" rel="stylesheet" type="text/css" media="screen" />
</head>

<body>
<tr><td style="width:9%"><img src="../picture/IIUM.PNG" width="310px" >
<div id="logo">
<head>
<head>
<title>Configuration-Items</title>
<link href="http://fonts.googleapis.com/css?family=Oswald" rel="stylesheet" type="text/css" />
<link href='http://fonts.googleapis.com/css?family=Arvo' rel='stylesheet' type='text/css'>
<link href="../css/style.css" rel="stylesheet" type="text/css" media="screen" />

</head>
							
<center><h2><a href="../configuration_items.html"><b>Configuration Items</a></h2></center>
<center><p><b>International Islamic University Malaysia</b></p></center>
<center><p><b>Information Technology Division</b></p></center>
</div>
<style>

body
{
	background:#CFF
}
</style>

<center><img src="../picture/itd_banner.jpg" width="960px" alt="" /></center>

<body>
		
        
					<div id="content">
					<div class="post">
					<form method="post" action="login.php">
					<h3 class="reel" align="center">Admin Login</h3>
					<div class="entry">
					<table width="300" border="0" align="center">
           <tr>
                <center><td>Username :</td>
				<td><input type="text" id="username" name="username"required>
				</td></center>
			</tr>
			<tr>
                <td><center>Password :</td>
				<td><input type="password" id="password" name="password"required>
				</td></center>
			</tr>
			<tr>
				<td><center>Category :</td>
				<td><select name="category" id="category">
				<option value="category">--</option>
				<option value="Admin" name="Admin">Admin</option>
				<option value="Gombak" name="Gombak">Gombak</option>
				<option value="Gambang" name="Gambang">Gambang</option>
				<option value="Indera Mahkota" name="Indera Mahkota">Indera Mahkota</option>
				<option value="Petaling Jaya" name="Petaling Jaya">Petaling Jaya</option>
				</select></center></td>
			</tr>
				<tr>
				<td><input class="myButton" type="submit" name="submit" value="Login"></td>
				 <td><input type="reset" name="button2" id="button2" value="Reset" /></td>
				</tr>
				</form>
            </div>
        </div>
      </div>
					<!-- clock -->					
<center><body>

<p id="ci"></p>

<script>
var myVar=setInterval(function(){myTimer()},1000);

function myTimer() {
    var d = new Date();
    document.getElementById("ci").innerHTML = d.toLocaleTimeString();
}
</script>
</center>
</body>
</html>
<!-- end clock -->

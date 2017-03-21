<html>
<head>
	<title>Objects, Local Storage</title>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
	<script>
	$(document).ready(function(){
        
        $("button").click(function() {
  			var nome = document.getElementById('objName');
            var num = document.getElementById('objNum');
            var code = document.getElementById('objCode');
            var bus = document.getElementById('objBus'); 
           document.write("New Client: " + nome.value + " #: " + num.value + " Area Code: "  + code.value + " Business: " + bus.value);
           
		});
	});
    
    
    
	</script>
	<style>
	body{
		background-color: rgb(90,120,250);
	}
	h1 {
		color: white;
	}
	p {
    	margin-left:50%;
		color:white;
	}
	box1 {
		height: 70px;
		width: 70px;
		border: 10px solid red;
	}
    
    button {
    	border-radius:3px;
        height:23px;
        width:70px;
        background-color:silver;
        margin-top:6%;
        margin-left:15%;
    }
	</style>
</head>
<body>

	

	<h1>Enter Client Info:</h1>
    <h3>Name: <input type="text" id="objName" value=""></h3>
    <h3>Phone Number: <input type="text" id="objNum" value=""></h3>
    <h3>Area Code: <input type="text" id="objCode" value=""></h3>
    <h3>Business: <input type="text" id="objBus" value=""></h3>
    
	<p></p>
	<button>Submit</button>
	<div id="box1"></div>
	<section id="result_display"></section>
</body>
</html>
<!doctype html>
<html>
<head>
	<title>Objects, Local Storage</title>
	<script>
		var objectOne = new Object();
        var objName = document.getElementById('objName').innerHTML;
        var objNum = document.getElementById('objNum').innerHTML;
        var objCode = document.getElementById('objCode').innerHTML;
        var objBus = document.getElementById('objBus').innerHTML;
        
        function submitClient(){
        
        	var result;
        	objectOne[objName];
            objectOne[objNum];
            objectOne[objCode];
            objectOne[objBus];
            
            console.log(objectOne);
            result = result.concat(objectOne.getOwnPropertyNames(objectOne));
            return result;
        }
	</script>
	<style>
	body{
		background-color: rgb(90,120,250);
	}
	h1 {
		color: white;
	}
	p {
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
    <h3>Name: <textarea id="objName"></textarea></h3>
    <h3>Phone Number: <textarea id="objNum"></textarea></h3>
    <h3>Area Code: <textarea id="objCode"></textarea></h3>
    <h3>Business: <textarea id="objBus"></textarea></h3>
    
	<p></p>
	<button id='submit' onclick='submitClient(this)'>Submit</button>
	<div id="box1"></div>
	<section id="result_display"></section>
</body>
</html>
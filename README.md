# To-do-List
My To-do-list
<html>

<title>To-do-list</title>

<head>

<div id="mytodolist" class="header">

  <h1>To Do List</h1>
  
</div>

<ol id="ol">

  <ol>
	
	   <li>Send a mail</li>
	   
	   <li>Call A Prospect</li>
	   
	   <li>Put finishing touches to my wordpress website</li>
	   
	   <li>Call my lawyer</li>
	   
	   <li>Respond to emails in my inbox</li>
	   
	   <li>Visit my Pastor</li>
	   
	   <li>Buy Groceries</li>
	
	</ol>


</head>



<body>
	
	<script type="text/javascript">
	
	var myNodelist = document.getElementsByTagName("LI");
    var i;
	for (i = 0; i < myNodelist.length; i++) {
	  var span = document.createElement("SPAN");
	  var txt = document.createTextNode;
	  span.className = "close";
	  span.appendChild(txt);
	  myNodelist[i].appendChild(span);
	}

	var close = document.getElementsByClassName("close");
	var i;
	for (i = 0; i < close.length; i++) {
	  close[i].onclick = function() {
		var div = this.parentElement;
		div.style.display = "none";
	  }
	}

	var list = document.querySelector('ol');

	function newElement() {
	  var li = document.createElement("li");
	  var inputValue = document.getElementById("myInput").value;
	  var t = document.createTextNode(inputValue);
	  li.appendChild(t);
	  if (inputValue === '') {
		alert("You must write something!");
	  } else {
		document.getElementById("ol").appendChild(li);
	  }
	  document.getElementById("myInput").value = "";

	  var span = document.createElement("SPAN");
	  var txt = document.createTextNode;
	  span.className = "close";
	  span.appendChild(txt);
	  li.appendChild(span);

	  for (i = 0; i < close.length; i++) {
		close[i].onclick = function() {
		  var div = this.parentElement;
		  div.style.display = "none";
		}
	  }
	}

	
	</script>

	
	</body>

















</html>

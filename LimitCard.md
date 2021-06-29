<script src="https://code.jquery.com/jquery-3.2.1.min.js"></script>

Here is your Limit:

<h><b><div id="limit">No Limit Yet</div></b></h>

<button id="btnClick">New Limit</button>
<script>
var limits = ["1-4", "5-6", "7+", "Adj/Adv", "Noun", "Verb", "AEIOUWY", "BP", "CSXZ", "FGHJKQV", "LRMN", "TD"]

$('#btnClick').on('click',function(){
document.getElementById("limit").innerHTML = limits[Math.floor(Math.random() * limits.length)];
});
</script>

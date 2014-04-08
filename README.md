GWD238_Lab1b
Continue to work with DOM; using forms to transform div objects.

<!doctype html>
<html>
<head>
<meta charset="UTF-8">
<title>Sydney Carter's Lab 1</title>

<style>
#circle{
    width: 100px;
    height: 100px;
    border-radius: 50%;
    border: 3px solid black;
    text-align: center;
}
</style>

</head>

<body>
<div id="circle">div2</div>

<form>
    <fieldset>
        <legend>Move Circle</legend>
        <input type="text" id="info" />
        <input type="button" id="button2" value="MOVE IT!" />
    </fieldset>
</form>

<script>
//CREATE SHORTCUT VARIABLES FOR DOM ELEMENTS
var circle = document.getElementById('circle')
var text = document.getElementById('info')
var button = document.getElementById('button2')

button.onclick = mover;

function mover(e) /*PLACE E INSIDE WHEN FUNCTION IS TRIGGERED BY EVENT HANDLER*/
{
    circle.style.marginLeft = text.value;    
}
</script>
</body>
</html>

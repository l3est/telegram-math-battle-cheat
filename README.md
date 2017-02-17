# telegram-math-battle-cheat
JavaScript code to cheat in math battle game.

just start the game and run the code on console : 
```javascript
var intervalId = setInterval(cheat, Math.floor(Math.random() * 100) + 200);

function cheat(){
var a = parseInt(document.getElementById("task_x").innerText);
var b = parseInt(document.getElementById("task_y").innerText);
var res = parseInt(document.getElementById("task_res").innerText); 
var operator = document.getElementById("task_op").innerText;
var btnC = document.getElementById("button_correct");
var btnR = document.getElementById("button_wrong");

switch(operator) {
    case "/":
        if( a / b == res)
			btnC.click();
		else
			btnR.click();
        break;
    case "+":
        if( a + b == res)
			btnC.click();
		else
			btnR.click();
        break;
	case "–":
        if( a - b == res)
			btnC.click();
		else
			btnR.click();
        break;
	case "×":
        if( a * b == res)
			btnC.click();
		else
			btnR.click();
        break;
}
};
```


to stop getting points run :
```javascript
clearInterval(intervalId);
```


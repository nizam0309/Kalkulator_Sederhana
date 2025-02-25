# Kalkulator_Sederhana
<!DOCTYPE html>
<html>
<head>
	<title>kalkulator</title>
</head>
<body>
<style>
	body{
		font-family: Arial, sans-serif;
			display: flex;
			justify-content: center;
			align-items: center;
			height: 100vh;
			background-color: blue;
	}
		.calculator {
			width: 300px;
			background-color: red;
			padding: 20px;
			border-radius: 10px;
			box-shadow: 0px 4px 6px rgba(0,0,0,0.1);
		}
		.calculator input {
			width: 100%;
			box-sizing: border-box;
			height: 40px;
			font-size: 20px;
			text-align: right;
			margin-bottom: 20px;
			padding: 10px;
			border-radius: 5px;
		}
		.buttons {
			display: grid;
			grid-template-columns: repeat(4, 1fr);
			gap: 8px;
		}
		.buttons button {
			background-color: white;
			font-size: 18px;
			padding: 20px;
			border-radius: 5px;
		}
		.buttons .hasil {
			grid-column: span 3;
		}
</style>
</head>
<body>
	<div class="calculator">
		<input type="text" id="display">
		<div class="buttons">
			<button onclick="appendToDisplay('1')">1</button>
			<button onclick="appendToDisplay('2')">2</button>
			<button onclick="appendToDisplay('3')">3</button>
			<button onclick="appendToDisplay('*')">x</button>
			<button onclick="appendToDisplay('4')">4</button>
			<button onclick="appendToDisplay('5')">5</button>
			<button onclick="appendToDisplay('6')">6</button>
			<button onclick="appendToDisplay('/')">/</button>
			<button onclick="appendToDisplay('7')">7</button>
			<button onclick="appendToDisplay('8')">8</button>
			<button onclick="appendToDisplay('9')">9</button>
			<button onclick="appendToDisplay('+')">+</button>
			<button onclick="appendToDisplay('0')">0</button>
			<button onclick="appendToDisplay('.')">.</button>
			<button onclick="ClearDisplay	(   )">AC</button>
			<button onclick="appendToDisplay('-')">-</button>
			<button class="hasil" onclick="calculateResult()">=</button>
			<button onclick="backspace()">C</button>
		</div>
			</body>
		</style>
	</div>
</div>
		<script>
		function appendToDisplay(value) {
			document.getElementById('display').value += value;
		}
		function ClearDisplay() {
			document.getElementById('display').value = '';
		}
		function backspace() {
			document.getElementById('display').value =display.value.slice(0, -1);
		}
		function calculateResult() {
			let display = document.getElementById('display').value;
			try {
				let result = eval (display);
				document.getElementById('display').value = result;
			} catch (error) {
				document.getElementById('display').value = 'Error Boss';
			}
		}
	</script>
</body>
</body>
</html>

<!DOCTYPE html>
<html>
    <head>
        <link href="/ANISH/ANISH.css/Calculator.css" rel="stylesheet" type="text/css">
        <meta charset="UTF-8">
        <title>Calculator</title>
    </head>
    <body>
        <div class="main">
        <form class="calculatorform" name="calculatorform">
            <div class="screen">
                <input type="text" name="screen" readonly>
            </div>
            <div class="btn">
                <input type="button" class="clearbtn" name="clear" value="Clear" onclick="Clear()">
            </div>
            <div class="btn">
                <input type="button" class="numbers" name="num1" value="1" onclick="valuebutton(this);">
                <input type="button" class="numbers" name="num2" value="2" onclick="valuebutton(this);">
                <input type="button" class="numbers" name="num3" value="3" onclick="valuebutton(this);">
                <input type="button" class="numbers" name="plus" value="+" onclick="valuebutton(this);">
            </div>
            <div class="btn">
                <input type="button" class="numbers" name="num4" value="4" onclick="valuebutton(this);">
                <input type="button" class="numbers" name="num5" value="5" onclick="valuebutton(this);">
                <input type="button" class="numbers" name="num6" value="6" onclick="valuebutton(this);">
                <input type="button" class="numbers" name="sub" value="-" onclick="valuebutton(this);">
            </div>
            <div class="btn">
                <input type="button" class="numbers" name="num7" value="7" onclick="valuebutton(this);">
                <input type="button" class="numbers" name="num8" value="8" onclick="valuebutton(this);">
                <input type="button" class="numbers" name="num9" value="9" onclick="valuebutton(this);">
                <input type="button" class="numbers" name="mul" value="*" onclick="valuebutton(this);">
            </div>
            <div class="btn">
                <input type="button" class="numbers" name="num0" value="0" onclick="valuebutton(this);">
                <input type="button" class="numbers" name="div" value="/" onclick="valuebutton(this);">
                <input type="button" class="numbers" name="equal" value="=" onclick="Calculate()">
             </div>
        </form>
        </div>
        <script>
            function valuebutton(e){
                calculatorform.screen.value += e.value
            }
            function Clear(){ 
                calculatorform.screen.value = null;
            }
            function Calculate(){
                calculatorform.screen.value = eval(calculatorform.screen.value)
            } 
        </script>
    </body>
</html>

# javascript-calculator
<!DOCTYPE html>
<html lang="en">
    <head>
<title>javascript calculator</title>

    </head>
<body>
    <table>
        <tr>
            <td><label>Enter first value</label>
            <input type="text" id="f_value" name="">
            </td>
            <td>
                <label>Enter second value</label>
                <input type="text" id="s_value" name="">
            </td>
            <td>
                <label>Result</label>
                <input type="text" id="Result" name="">
            </td>
        </tr>
    </table>
    <input type="button" id="add" value="Addition" 
    onclick="calculate(1);" name="">
    <input type="button" id="sub" value="Subtraction" 
    onclick="calculate(2);" name="">
    <input type="button" id="mul" value="Multiplication" 
    onclick="calculate(3);" name="">
    <input type="button" id="div" value="Division" 
    onclick="calculate(4);" name="">
    <script type="text/javascript">
        function calculate(choice) {
            var n1 = document.getElementById("f_value").value * 1;
            var n2 = document.getElementById("s_value").value * 1;
            var fresult;
            switch(choice) {
                case 1:
                    fresult = n1 + n2;
                    break;
                case 2:
                    fresult = n1 - n2;
                    break;
                case 3:
                    fresult = n1 * n2;
                    break;
                case 4:
                    fresult = n1 / n2;
                    break;
            }
            document.getElementById("Result").value = fresult;
        }
    </script>
</body>
</html>

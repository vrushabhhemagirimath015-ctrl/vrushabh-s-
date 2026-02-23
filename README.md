# vrushabh-s-
web page development

<!DOCTYPE html>
<html>
<head>
    <title>Fruit Shop</title>
    <script>
        function calculateTotal() {
            let total = 0;

            if(document.getElementById("apple").checked)
                total += 200;

            if(document.getElementById("orange").checked)
                total += 180;

            if(document.getElementById("banana").checked)
                total += 80;

            let tax = total * 0.10;
            let finalTotal = total + tax;

            alert("Your total cost is Rs. " + finalTotal);
        }
    </script>
</head>
<body>
    <h2>Fruit Selection</h2>

    <form>
        <input type="checkbox" id="apple"> Apple (Rs. 200/kg) <br><br>
        <input type="checkbox" id="orange"> Orange (Rs. 180/kg) <br><br>
        <input type="checkbox" id="banana"> Banana (Rs. 80/kg) <br><br>

        <input type="button" value="Calculate Total" onclick="calculateTotal()">
    </form>
</body>
</html>

<!DOCTYPE html>
<html>
<head>
    <title>Height Converter</title>
</head>
<body>

    <h2>Height Converter (Feet to CM)</h2>

    <label>Enter height in feet:</label>
    <input type="number" id="feet" step="0.01">
    <br><br>

    <button onclick="convert()">Convert</button>
    <br><br>

    <p id="result"></p>

    <script>
        function convert() {
            let feet = document.getElementById("feet").value;
            let cm = feet * 30.48;
            document.getElementById("result").innerHTML =
                "Height in centimeters: " + cm.toFixed(2) + " cm";
        }
    </script>

</body>
</html>

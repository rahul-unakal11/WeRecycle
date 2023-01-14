# WeRecycle
<!DOCTYPE html>
<html>
<head>
    <title>Recyclable</title>
    <style>
        body {
            background-color: #FFA07A; /* Light salmon */
        }
        .container {
            background-color: #FF4500; /* Orange-red */
            padding: 20px;
            border-radius: 10px;
            margin: 0 auto;
            width: 80%;
        }
        h1 {
            text-align: center;
            color: white;
        }
        form {
            margin-top: 20px;
            text-align: center;
        }
        input {
            margin: 10px;
            padding: 5px;
            border-radius: 5px;
            border: none;
        }
        button {
            background-color: #4CAF50; /* Green */
            color: white;
            padding: 10px 20px;
            border-radius: 5px;
            border: none;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Contact Us</h1>
        <form>
            <input type="text" placeholder="Name" id="name"><br>
            <input type="text" placeholder="Address" id="address"><br>
            <input type="text" placeholder="Phone Number" id="phoneNumber"><br>
            <button onclick="submitForm()">Submit</button>
        </form>
    </div>
    <script>
        function submitForm() {
            var name = document.getElementById("name").value;
            var address = document.getElementById("address").value;
            var phoneNumber = document.getElementById("phoneNumber").value;
            alert("Thank you for using our app, " + name + "! We will contact you shortly to schedule a collection at " + address + " . The phone number provided by you is " + phoneNumber + ".");
            // Send the data to the server
            // ...
        }
    </script>
</body>
</html>

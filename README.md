```html

<!DOCTYPE html>

<html>

<head>

&#x20;   <title>Bank Management System</title>

&#x20;   <link rel="stylesheet" href="style.css">

</head>

<body>



&#x20;   <h1>Welcome to Bank Management System</h1>



&#x20;   <h2>Customer Details</h2>



&#x20;   <p>Account Holder: Rahul</p>

&#x20;   <p>Account Number: 123456789</p>

&#x20;   <p>Account Type: Savings</p>



&#x20;   <h2>Banking Services</h2>



&#x20;   <button onclick="checkBalance()">Check Balance</button>

&#x20;   <button onclick="deposit()">Deposit</button>

&#x20;   <button onclick="withdraw()">Withdraw</button>



&#x20;   <h3 id="result">Balance: Rs. 10000</h3>



&#x20;   <script>

&#x20;       let balance = 10000;



&#x20;       function checkBalance() {

&#x20;           document.getElementById("result").innerHTML =

&#x20;               "Current Balance: Rs. " + balance;

&#x20;       }



&#x20;       function deposit() {

&#x20;           let amount = Number(prompt("Enter deposit amount:"));

&#x20;           if (amount > 0) {

&#x20;               balance += amount;

&#x20;               checkBalance();

&#x20;           } else {

&#x20;               alert("Enter a valid amount");

&#x20;           }

&#x20;       }



&#x20;       function withdraw() {

&#x20;           let amount = Number(prompt("Enter withdrawal amount:"));

&#x20;           if (amount > 0 \&\& amount <= balance) {

&#x20;               balance -= amount;

&#x20;               checkBalance();

&#x20;           } else {

&#x20;               alert("Invalid amount or insufficient balance");

&#x20;           }

&#x20;       }

&#x20;   </script>



</body>

</html>

```


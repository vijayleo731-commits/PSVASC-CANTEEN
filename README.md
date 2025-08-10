# PSVASC-CANTEEN
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Token System</title>
    <link rel="stylesheet" href="style.css">
  {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

body {
    background: linear-gradient(120deg, #ffecd2, #fcb69f);
    color: #333;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
}

header {
    background: #ff7043;
    color: white;
    text-align: center;
    padding: 20px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}

header h1 {
    font-size: 2rem;
}

main {
    flex: 1;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    padding: 20px;
    gap: 30px;
}

.form-container, .token-list {
    background: white;
    padding: 20px;
    border-radius: 15px;
    width: 300px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.1);
}

h2 {
    text-align: center;
    margin-bottom: 15px;
}

input, select, button {
    width: 100%;
    padding: 10px;
    margin: 8px 0;
    border-radius: 8px;
    border: 1px solid #ccc;
    font-size: 1rem;
}

button {
    background: #ff7043;
    color: white;
    border: none;
    cursor: pointer;
    font-weight: bold;
    transition: 0.3s;
}

button:hover {
    background: #ff5722;
}

ul {
    list-style: none;
}

ul li {
    padding: 10px;
    background: #ffe0b2;
    margin: 5px 0;
    border-radius: 8px;
    animation: fadeIn 0.5s ease-in-out;
}

@keyframes fadeIn {
    from {opacity: 0; transform: translateY(10px);}
    to {opacity: 1; transform: translateY(0);}
}

footer {
    background: #ff7043;
    color: white;
    text-align: center;
    padding: 10px;
}

</head>
<body>
    <header>
        <h1>PSVAS College Canteen Food Token System</h1>
    </header>

    <main>
        <section class="order-section">
            <h2>Place Your Order</h2>
            <form id="orderForm">
                <label for="studentName">Student Name:</label>
                <input type="text" id="studentName" required>

                 <label for="student class">Student class:</label>
                <input type="text" id="student class" required>

                <label for="foodItem">Select Food Item:</label>
                <select id="foodItem" required>
                    <option value="">BREAKFAST menu</option>
                    <option value="Idli - ₹8">Idli - ₹8</option>
                    <option value="Dosa - ₹20">Dosa - ₹20</option>
                    <option value="Poori - ₹15">Poori - ₹15</option>
                    <option value="Tea - ₹10">Tea - ₹10</option>
                    <option value="Coffee - ₹15">Coffee - ₹15</option>
                     <option value="">LUNCH menu</option>
                    <option value="veg rice - ₹60">veg rice - ₹60</option>
                    <option value="chicken rice - ₹80">chicken rice - ₹80</option>
                    <option value="chicken briyani - ₹100">chicken briyani - ₹100</option>
                    <option value="sambar satham - ₹50">sambar satham - ₹50</option>
                    <option value="curd rice- ₹40">curd rice- ₹40</option>
                </select>
                

                <button type="submit">Generate Token</button>
            </form>
        </section>

        <section class="token-section">
            <h2>Issued Tokens</h2>
            <table>
                <thead>
                    <tr>
                        <th>Token No</th>
                        <th>Student Name</th>
                         <th>Student class</th>
                        <th>Food Item</th>
                        <th>Time</th>
                    </tr>
                </thead>
                <tbody id="tokenList">
                </tbody>
            </table>
        </section>
    </main>

    <footer>
        <p>© 2025 PSVAS College Canteen Token System</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

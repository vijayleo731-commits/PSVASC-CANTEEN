# PSVASC-CANTEEN
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Token System</title>
    <link rel="stylesheet" href="style.css">
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

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Our Menu</title>
    <link rel="stylesheet" href="styles1.css"> <!-- Link to external CSS file -->
</head>
<body>
    <header>
        <h1>Our Menu</h1>
    </header>
    <div class="container">
        <div class="menu">
            <div class="menu-item">
                <div class="heading-box">
                    <h2>Starters</h2>
                </div>
                <p>A selection of delicious appetizers to begin your meal.</p>
            </div>
            <div class="menu-item">
                <div class="heading-box">
                    <h2>Main Course</h2>
                </div>
                <p>Our signature dishes designed to satisfy your main cravings.</p>
            </div>
            <div class="menu-item">
                <div class="heading-box">
                    <h2>Desserts</h2>
                </div>
                <p>Indulge yourself with our decadent sweet treats to finish off.</p>
            </div>
        </div>
    </div>
    
</body>
</html>


/* Seperate Style Sheet styles1.css */

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

header {
    background: #333;
    color: #fff;
    padding: 20px;
    text-align: center;
}

.container {
    width: 90%;
    margin: auto;
    overflow: hidden;
}

.menu {
    display: flex;
    justify-content: space-between;
    margin-top: 20px;
}

.menu-item {
    background: lightpink;
    border-radius: 5px;
    padding: 20px;
    flex: 1; /* Allowing each item to grow equally */
    margin: 10px; 
    text-align: center;
    transition: transform 0.2s;
    margin-bottom: 20px; 
}

.menu-item:hover {
    transform: scale(1.05);
}

.menu-item .heading-box {
    background-color: #333; 
    color: white; 
    padding: 10px; 
    border-radius: 5px; /* Rounded corners */
    text-align: right; 
    margin-bottom: 10px; 
}

.menu-item h2 {
    margin: 0; /* Reset margin */
    font-size: 1.5em; /* Heading size */
}

.menu-item p {
    color: #666;
}


/* Mobile Styles(small devices) */
@media (max-width: 600px) {
    .menu {
        flex-direction: column; /* Stack items on top of each other */
    }
    .menu-item {
        flex: 1 1 100%; /* Full width for mobile */
        margin: 5px ; /* Adjust margin for vertical stacking */
    }
}

/* Tablet Styles(medium devices) */
@media (min-width: 601px) and (max-width: 900px) {
    .menu-item {
        flex: 1 1 100%; 
        margin: 10px; 
    }
}

/* Desktop Styles(large devices) */
@media (min-width: 901px) {
    .menu-item {
        flex: 1 1 30%; 
        margin: 10px; 
    }
}

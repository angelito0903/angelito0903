function doGet(e) {
    return HtmlService.createHtmlOutputFromFile('dashboard')
        .setTitle('My Dashboard');
}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Dashboard</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background-color: white;
            height: 100vh;
        }
        .dashboard-title {
            font-size: 36px;
            font-weight: bold;
            text-align: center;
            margin-bottom: 20px;
        }
        .dashboard-frame {
            width: 1800px;
            height: 800px;
            border: 2px solid black;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 20px;
            background-color: #ffffff;
        }
        .sub-menu {
            width: 1200px;
            height: 100px;
            background-color: red;
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 10px;
            border-radius: 5px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            transition: transform 0.2s, box-shadow 0.2s;
            cursor: pointer;
        }
        .sub-menu:active {
            transform: translateY(4px);
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
        }
    </style>
</head>
<body>
    <div class="dashboard-title">MY DASHBOARD</div>
    <div class="dashboard-frame">
        <a href="accounting.html" class="sub-menu">Accounting</a>
        <div class="sub-menu">Sales</div>
        <div class="sub-menu">Product Update</div>
        <div class="sub-menu">Product Development</div>
        <div class="sub-menu">Inquiry</div>
        <div class="sub-menu">Manufacturing</div>
    </div>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Accounting</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: white;
            height: 100vh;
        }
        .accounting-frame {
            width: 1800px;
            height: 800px;
            border: 2px solid black;
            display: flex;
            background-color: #ffffff;
        }
        .sidebars {
            display: flex;
            flex-direction: column;
            width: 50px;
            height: 500px;
            margin: auto 0;
            background-color: red;
            color: white;
            text-align: center;
            font-size: 14px;
            padding: 10px 5px;
            justify-content: space-evenly;
            align-items: center;
        }
        .sidebar-item {
            background-color: red;
            color: white;
            width: 50px;
            height: 50px;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 5px 0;
            border-radius: 5px;
            font-size: 12px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="accounting-frame">
        <div class="sidebars">
            <div class="sidebar-item">Cash</div>
            <div class="sidebar-item">Request</div>
            <div class="sidebar-item">Receivable</div>
            <div class="sidebar-item">Payable</div>
        </div>
        <div style="flex-grow: 1; text-align: center; padding: 20px;">
            <h1>Welcome to the Accounting Page</h1>
        </div>
    </div>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Expanding Card</title>
    <style>
        *{
            box-sizing: border-box;
            margin: 0;;
            padding: 0;
        }

        body{
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: rgb(1, 33, 33);
            font-family: Arial, Helvetica, sans-serif;
        }

        .container{
            display: flex;
            gap: 15px;
        }

        .card{
            background-color: #504d4d;
            width: 150px; 
            height: 150px;
            transition: all 0.3s ease;
            border-radius: 10px;
            overflow: hidden;
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
            position: relative;
            text-align: center;
        }

        .card:hover{
            width: 200px;
            height: 200px;
            background-color: #555;
        }

        .card .content{
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .card:hover .content{
            opacity: 1;
        }

        .card .title{
            font-size: 1.5em;
            font-weight: bold;
        }

        .card .decription{
            font-size: 1em;
            opacity: 0;
        }
        .card:hover .decription{
            opacity: 1;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="card">
            <div class="content">  
                <div class="title">Card-1</div>
                <div class="decription">More Info</div>
            </div>
        </div>
        <div class="card">
            <div class="content">
                <div class="title">Card-2</div>
                <div class="decription">More Info</div>
            </div>
        </div>
        <div class="card">
            <div class="content">
                <div class="title">Card-3</div>
                <div class="decription">More Info</div>
            </div>
        </div>
    </div>
</body>
</html>

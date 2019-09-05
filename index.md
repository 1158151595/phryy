<!DOCTYPE html>

<html lang="en">
<head>
    <meta charset="UTF-8" />
    <title>个人主页</title>
    <script type="text/javascript" src="js/jquery-1.9.1.min.js"></script>
    <script type="text/javascript" src="js/util/pdfobject.js"></script>
    <script type="text/javascript" src="js/index.js"></script>
    <style type="text/css">
        .redBall{
            color: red;
        }
        .blueBall{
            color: blue;
        }
    </style>
</head>
<body style="height: 100%;width: 100%;">
<div style="width: 600px;height: 50px;margin: 10px auto;">
    <table style="width: 600px;text-align: center;">
       <tr>
           <td><a href="index">首页</a></td>
           <td><a href="randomtest">测试机选</a></td>
           <td><a href="test">测试算法</a></td>
           <td><a href="forecast">往期预测结果</a></td>
       </tr>
    </table>
</div>
<div style="width: 600px;height: 400px;border: 1px gainsboro solid;margin: 20px auto;">
    <span>系统随机生成的五注双色球</span><br />
    <div id="forecastShow">
        <span id="num">期号：</span>
        <table style="width: 600px;height: 380px;text-align: center;">
            <thead align="center !important">
                <tr>
                    <th>红球</th>
                    <th>蓝球</th>
                    <th>中奖等级</th>
                </tr>
            </thead>
            <tbody id="ballsBody">

            </tbody>
        </table>
    </div>
    <div id="chooseDiv">
        <table style="width: 600px;height: 400px;text-align: center;">
            <tr>
                <td class="redBall">红球杀号</td>
                <td><input type="text" id="redKill" /></td>
                <td class="blueBall">蓝球杀号</td>
                <td><input type="text" id="blueKill" /></td>
            </tr>
            <tr>
                <td class="redBall">红球最小</td>
                <td><input type="text" id="redMin" /></td>
                <td class="redBall">红球最大</td>
                <td><input type="text" id="redMax" /></td>
            </tr>
            <tr>
                <td class="blueBall">蓝球最小</td>
                <td><input type="text" id="blueMin" /></td>
                <td class="blueBall">蓝球最大</td>
                <td><input type="text" id="blueMax" /></td>
            </tr>
        </table>
        <button onclick="getForecast()">确定</button>
    </div>
</div>
</body>
</html>

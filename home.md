由于笔者大一过去一年的学习和竞赛之路十分坎坷,加之各方原因,所以纯粹是为爱发电,编写了此手册.希望能够给海南师范大学信息科学技术学院的学生带来帮助.同时宣传一下双创与学科教育竞赛指导中心(手册其他部分简称竞赛中心).

__手册中大部分回答仅代表个人观点，不涉及其他个人及组织__

添加更多Part的建议请发送至以下邮箱: ```freak050321@gmail.com```

样例如下：
```
收件人:freak050321@gmail.com

主题:手册<Part>——具体来意

正文:略
```
<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>计时器</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
            text-align: center;
        }
        .timer {
            font-size: 2em;
            color: #333;
        }
    </style>
</head>
<body>
    <div class="timer" id="timer">计时器</div>

<script>
        // 设置开始时间
        const startTime = new Date('2024-10-22T21:00:00Z').getTime();

        function updateTimer() {
            const now = new Date().getTime();
            const elapsedTime = now - startTime; // 计算已经过去的时间

            // 计算天、小时、分钟和秒
            const days = Math.floor(elapsedTime / (1000 * 60 * 60 * 24));
            const hours = Math.floor((elapsedTime % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((elapsedTime % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((elapsedTime % (1000 * 60)) / 1000);

            // 更新页面显示
            document.getElementById('timer').innerHTML = `${days}天 ${hours}时 ${minutes}分 ${seconds}秒`;
        }

        // 每秒更新一次计时器
        setInterval(updateTimer, 1000);
</script>
</body>
</html>

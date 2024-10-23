<div id="timer" style="font-size: 2em; color: #333; text-align: center;">test</div>

```eval-js
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
```

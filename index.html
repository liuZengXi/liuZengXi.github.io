<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>周五下班倒计时</title>
    <link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>⏰</text></svg>">
    <style>
        :root {
            --primary: #3498db;
            --secondary: #2980b9;
            --accent: #e74c3c;
            --light: #ecf0f1;
            --dark: #2c3e50;
            --success: #2ecc71;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background: linear-gradient(135deg, #1a2a6c, #b21f1f, #fdbb2d);
            padding: 20px;
            color: #333;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 800px;
            width: 100%;
            text-align: center;
        }
        
        .header {
            margin-bottom: 30px;
            color: white;
            text-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
        }
        
        .header h1 {
            font-size: 2.8rem;
            margin-bottom: 10px;
        }
        
        .header p {
            font-size: 1.2rem;
            opacity: 0.9;
        }
        
        .card {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            padding: 40px 30px;
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
            backdrop-filter: blur(10px);
            margin-bottom: 30px;
            animation: fadeIn 1s ease;
            border: 1px solid rgba(255, 255, 255, 0.3);
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .countdown {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin: 30px 0;
        }
        
        .time-unit {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 25px 15px;
            border-radius: 15px;
            min-width: 140px;
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }
        
        .time-unit::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: rgba(255, 255, 255, 0.5);
        }
        
        .time-unit:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 20px rgba(0, 0, 0, 0.15);
        }
        
        .time-value {
            font-size: 3.5rem;
            font-weight: 700;
            margin-bottom: 5px;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
        }
        
        .time-label {
            font-size: 1.2rem;
            opacity: 0.9;
            font-weight: 500;
        }
        
        .message {
            margin-top: 20px;
            font-size: 1.3rem;
            color: var(--dark);
            line-height: 1.6;
        }
        
        .highlight {
            color: var(--accent);
            font-weight: 600;
        }
        
        .weekend-info {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 15px;
            padding: 25px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
            backdrop-filter: blur(10px);
            animation: fadeIn 1s ease 0.2s both;
            border: 1px solid rgba(255, 255, 255, 0.3);
        }
        
        .weekend-info h2 {
            color: var(--dark);
            margin-bottom: 20px;
            font-size: 1.8rem;
        }
        
        .progress-container {
            background: var(--light);
            border-radius: 10px;
            height: 20px;
            margin: 20px 0;
            overflow: hidden;
            box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.2);
        }
        
        .progress-bar {
            height: 100%;
            background: linear-gradient(90deg, var(--success), #27ae60);
            width: 0%;
            transition: width 0.5s ease;
            border-radius: 10px;
        }
        
        .week-stats {
            display: flex;
            justify-content: space-around;
            margin-top: 20px;
            font-size: 1rem;
        }
        
        .stat {
            padding: 10px;
        }
        
        .stat-value {
            font-weight: 700;
            font-size: 1.5rem;
            color: var(--primary);
        }
        
        .motivation {
            margin-top: 20px;
            font-style: italic;
            color: #7f8c8d;
        }
        
        .floating {
            position: absolute;
            width: 60px;
            height: 60px;
            background: rgba(255, 255, 255, 0.15);
            border-radius: 50%;
            animation: float 20s infinite linear;
            z-index: -1;
        }
        
        @keyframes float {
            0% { transform: translate(0, 0) rotate(0deg); }
            25% { transform: translate(100px, 100px) rotate(90deg); }
            50% { transform: translate(50px, 200px) rotate(180deg); }
            75% { transform: translate(-50px, 100px) rotate(270deg); }
            100% { transform: translate(0, 0) rotate(360deg); }
        }
        
        @media (max-width: 600px) {
            .header h1 {
                font-size: 2rem;
            }
            
            .time-unit {
                min-width: 110px;
                padding: 20px 10px;
            }
            
            .time-value {
                font-size: 2.5rem;
            }
            
            .countdown {
                gap: 10px;
            }
        }
        
        .github-info {
            margin-top: 20px;
            color: white;
            font-size: 0.9rem;
            opacity: 0.8;
        }
        
        .github-info a {
            color: white;
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <!-- 浮动背景元素 -->
    <div class="floating" style="top: 10%; left: 5%; animation-delay: 0s;"></div>
    <div class="floating" style="top: 20%; left: 80%; animation-delay: -5s;"></div>
    <div class="floating" style="top: 70%; left: 10%; animation-delay: -10s;"></div>
    <div class="floating" style="top: 80%; left: 70%; animation-delay: -15s;"></div>
    
    <div class="container">
        <div class="header">
            <h1>周五下班倒计时</h1>
            <p>实时显示距离周末还有多久</p>
        </div>
        
        <div class="card">
            <h2>距离周五18:00下班还有</h2>
            <div class="countdown">
                <div class="time-unit">
                    <div class="time-value" id="hours">00</div>
                    <div class="time-label">小时</div>
                </div>
                <div class="time-unit">
                    <div class="time-value" id="minutes">00</div>
                    <div class="time-label">分钟</div>
                </div>
                <div class="time-unit">
                    <div class="time-value" id="seconds">00</div>
                    <div class="time-label">秒</div>
                </div>
            </div>
            <div class="message">
                坚持就是胜利！距离周末还有 <span class="highlight" id="total-hours">0</span> 小时
            </div>
            <div class="motivation" id="motivation-text">加油，您已经做得很棒了！</div>
        </div>
        
        <div class="weekend-info">
            <h2>本周工作进度</h2>
            <div class="progress-container">
                <div class="progress-bar" id="week-progress"></div>
            </div>
            <div class="week-stats">
                <div class="stat">
                    <div class="stat-value" id="week-passed">0</div>
                    <div>已过去</div>
                </div>
                <div class="stat">
                    <div class="stat-value" id="week-remaining">5</div>
                    <div>工作日剩余</div>
                </div>
                <div class="stat">
                    <div class="stat-value" id="week-percentage">0%</div>
                    <div>完成度</div>
                </div>
            </div>
            <div class="motivation" id="week-status">新的一周刚刚开始！</div>
        </div>
        
        <div class="github-info">
            <p>本页面使用 GitHub Pages 部署 | <a href="https://github.com/yourusername/your-repo" target="_blank">查看源代码</a></p>
        </div>
    </div>

    <script>
        // 励志语句库
        const motivations = [
            "加油，您已经做得很棒了！",
            "坚持就是胜利！",
            "每一天都是新的开始！",
            "您离周末又近了一步！",
            "保持专注，时间会过得很快！",
            "完成工作后就可以享受周末了！",
            "您正在进步，继续保持！",
            "今天也是努力工作的一天！"
        ];
        
        function updateCountdown() {
            const now = new Date();
            const currentDay = now.getDay(); // 0是周日，1是周一，...，5是周五
            const currentHour = now.getHours();
            const currentMinute = now.getMinutes();
            const currentSecond = now.getSeconds();
            
            // 计算下一个周五18:00
            let daysUntilFriday;
            if (currentDay < 5) {
                // 如果是周一到周四
                daysUntilFriday = 5 - currentDay;
            } else if (currentDay === 5 && currentHour < 18) {
                // 如果是周五但还没到18:00
                daysUntilFriday = 0;
            } else {
                // 如果是周五18:00后或周末
                daysUntilFriday = 5 - currentDay + 7;
            }
            
            // 计算目标时间
            const targetTime = new Date(now);
            targetTime.setDate(now.getDate() + daysUntilFriday);
            targetTime.setHours(18, 0, 0, 0);
            
            // 计算时间差
            const timeDiff = targetTime - now;
            
            // 如果已经是周五18:00或之后，显示0
            if (timeDiff <= 0) {
                document.getElementById('hours').textContent = '00';
                document.getElementById('minutes').textContent = '00';
                document.getElementById('seconds').textContent = '00';
                document.getElementById('total-hours').textContent = '0';
                document.getElementById('motivation-text').textContent = "周末到了，好好享受吧！";
                return;
            }
            
            // 计算总小时数（包括天数转换的小时）
            const totalHours = Math.floor(timeDiff / (1000 * 60 * 60));
            
            // 计算小时、分钟、秒（只显示小时、分钟和秒）
            const hours = Math.floor(timeDiff / (1000 * 60 * 60));
            const minutes = Math.floor((timeDiff % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((timeDiff % (1000 * 60)) / 1000);
            
            // 更新倒计时显示
            document.getElementById('hours').textContent = hours.toString().padStart(2, '0');
            document.getElementById('minutes').textContent = minutes.toString().padStart(2, '0');
            document.getElementById('seconds').textContent = seconds.toString().padStart(2, '0');
            
            // 显示总小时数
            document.getElementById('total-hours').textContent = totalHours;
            
            // 随机显示励志语句
            if (seconds % 30 === 0) {
                const randomIndex = Math.floor(Math.random() * motivations.length);
                document.getElementById('motivation-text').textContent = motivations[randomIndex];
            }
            
            // 更新周进度
            updateWeekProgress(now);
        }
        
        function updateWeekProgress(now) {
            const currentDay = now.getDay();
            const currentHour = now.getHours();
            
            // 计算本周已过去的工作日
            let weekPassed = 0;
            let weekStatus = "";
            
            if (currentDay >= 1 && currentDay <= 5) {
                weekPassed = currentDay - 1;
                if (currentHour >= 18) {
                    weekPassed += 1;
                }
                
                // 设置状态消息
                if (weekPassed === 0) {
                    weekStatus = "新的一周刚刚开始！";
                } else if (weekPassed === 1) {
                    weekStatus = "周一已经过去，继续加油！";
                } else if (weekPassed === 2) {
                    weekStatus = "周二也结束了，坚持就是胜利！";
                } else if (weekPassed === 3) {
                    weekStatus = "周三已过，周末越来越近了！";
                } else if (weekPassed === 4) {
                    weekStatus = "周四即将结束，明天就是周五了！";
                } else if (weekPassed === 5) {
                    weekStatus = "周五到了，今天就能解放了！";
                }
            } else if (currentDay === 0 || currentDay === 6) {
                weekPassed = 5; // 周末显示为已完成
                weekStatus = "享受您的周末时光！";
            }
            
            // 计算本周剩余工作日
            let weekRemaining = 5 - weekPassed;
            if (weekRemaining < 0) weekRemaining = 0;
            
            // 计算周进度百分比
            const weekPercentage = Math.round((weekPassed / 5) * 100);
            
            // 更新显示
            document.getElementById('week-passed').textContent = weekPassed;
            document.getElementById('week-remaining').textContent = weekRemaining;
            document.getElementById('week-percentage').textContent = `${weekPercentage}%`;
            document.getElementById('week-progress').style.width = `${weekPercentage}%`;
            document.getElementById('week-status').textContent = weekStatus;
        }
        
        // 初始加载
        updateCountdown();
        
        // 每秒更新一次
        setInterval(updateCountdown, 1000);
    </script>
</body>
</html>

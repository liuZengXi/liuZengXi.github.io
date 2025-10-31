<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>自定义下班倒计时</title>
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
            margin-bottom: 20px;
            color: white;
            text-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
        }
        
        .header h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }
        
        .header p {
            font-size: 1.1rem;
            opacity: 0.9;
        }
        
        .card {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            padding: 30px 25px;
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
            backdrop-filter: blur(10px);
            margin-bottom: 20px;
            animation: fadeIn 1s ease;
            border: 1px solid rgba(255, 255, 255, 0.3);
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .settings {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 15px;
            padding: 20px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
            backdrop-filter: blur(10px);
            margin-bottom: 20px;
            animation: fadeIn 1s ease 0.2s both;
            border: 1px solid rgba(255, 255, 255, 0.3);
        }
        
        .settings h2 {
            color: var(--dark);
            margin-bottom: 15px;
            font-size: 1.5rem;
        }
        
        .setting-group {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            justify-content: center;
            margin-bottom: 15px;
        }
        
        .setting-item {
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            flex: 1;
            min-width: 180px;
        }
        
        label {
            font-weight: 600;
            margin-bottom: 6px;
            color: var(--dark);
            font-size: 0.9rem;
        }
        
        input, select {
            width: 100%;
            padding: 10px 12px;
            border: 2px solid #ddd;
            border-radius: 8px;
            font-size: 0.9rem;
            transition: all 0.3s;
        }
        
        input:focus, select:focus {
            border-color: var(--primary);
            outline: none;
            box-shadow: 0 0 0 3px rgba(52, 152, 219, 0.2);
        }
        
        .quick-buttons {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            justify-content: center;
            margin-top: 15px;
        }
        
        .btn {
            padding: 8px 16px;
            background: var(--primary);
            color: white;
            border: none;
            border-radius: 8px;
            font-size: 0.9rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        
        .btn:hover {
            background: var(--secondary);
            transform: translateY(-2px);
            box-shadow: 0 6px 8px rgba(0, 0, 0, 0.15);
        }
        
        .btn-secondary {
            background: #95a5a6;
        }
        
        .btn-secondary:hover {
            background: #7f8c8d;
        }
        
        .countdown {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
            margin: 25px 0;
        }
        
        .time-unit {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 20px 15px;
            border-radius: 12px;
            min-width: 120px;
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
            height: 3px;
            background: rgba(255, 255, 255, 0.5);
        }
        
        .time-unit:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 20px rgba(0, 0, 0, 0.15);
        }
        
        .time-value {
            font-size: 2.8rem;
            font-weight: 700;
            margin-bottom: 5px;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.2);
        }
        
        .time-label {
            font-size: 1rem;
            opacity: 0.9;
            font-weight: 500;
        }
        
        .message {
            margin-top: 15px;
            font-size: 1.1rem;
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
            padding: 20px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
            backdrop-filter: blur(10px);
            animation: fadeIn 1s ease 0.4s both;
            border: 1px solid rgba(255, 255, 255, 0.3);
        }
        
        .weekend-info h2 {
            color: var(--dark);
            margin-bottom: 15px;
            font-size: 1.5rem;
        }
        
        .progress-container {
            background: var(--light);
            border-radius: 8px;
            height: 16px;
            margin: 15px 0;
            overflow: hidden;
            box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.2);
        }
        
        .progress-bar {
            height: 100%;
            background: linear-gradient(90deg, var(--success), #27ae60);
            width: 0%;
            transition: width 0.5s ease;
            border-radius: 8px;
        }
        
        .week-stats {
            display: flex;
            justify-content: space-around;
            margin-top: 15px;
            font-size: 0.9rem;
        }
        
        .stat {
            padding: 8px;
        }
        
        .stat-value {
            font-weight: 700;
            font-size: 1.3rem;
            color: var(--primary);
        }
        
        .motivation {
            margin-top: 15px;
            font-style: italic;
            color: #7f8c8d;
            font-size: 0.9rem;
        }
        
        .floating {
            position: absolute;
            width: 50px;
            height: 50px;
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
        
        @media (max-width: 768px) {
            .header h1 {
                font-size: 2rem;
            }
            
            .time-unit {
                min-width: 100px;
                padding: 15px 10px;
            }
            
            .time-value {
                font-size: 2.2rem;
            }
            
            .countdown {
                gap: 10px;
            }
            
            .setting-group {
                flex-direction: column;
            }
            
            .setting-item {
                min-width: 100%;
            }
        }
        
        .github-info {
            margin-top: 15px;
            color: white;
            font-size: 0.8rem;
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
            <h1>自定义下班倒计时</h1>
            <p>设置您自己的目标时间，实时查看倒计时</p>
        </div>
        
        <div class="settings">
            <h2>设置目标时间</h2>
            <div class="setting-group">
                <div class="setting-item">
                    <label for="target-date">目标日期</label>
                    <input type="date" id="target-date">
                </div>
                <div class="setting-item">
                    <label for="target-time">目标时间</label>
                    <input type="time" id="target-time" value="18:00">
                </div>
            </div>
            <div class="quick-buttons">
                <button class="btn" id="friday-btn">本周五 18:00</button>
                <button class="btn" id="today-btn">今天 18:00</button>
                <button class="btn btn-secondary" id="reset-btn">重置</button>
            </div>
        </div>
        
        <div class="card">
            <h2>距离目标时间还有</h2>
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
                目标时间: <span class="highlight" id="target-display">未设置</span>
            </div>
            <div class="motivation" id="motivation-text">请设置目标时间开始倒计时</div>
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
            <p>本页面使用 GitHub Pages 部署 | <a href="#" id="github-link">查看源代码</a></p>
        </div>
    </div>

    <script>
        // 励志语句库
        const motivations = [
            "加油，您已经做得很棒了！",
            "坚持就是胜利！",
            "每一天都是新的开始！",
            "您离目标又近了一步！",
            "保持专注，时间会过得很快！",
            "完成工作后就可以放松了！",
            "您正在进步，继续保持！",
            "今天也是努力工作的一天！"
        ];
        
        // 目标时间变量
        let targetDateTime = null;
        
        // DOM 元素
        const targetDateInput = document.getElementById('target-date');
        const targetTimeInput = document.getElementById('target-time');
        const fridayBtn = document.getElementById('friday-btn');
        const todayBtn = document.getElementById('today-btn');
        const resetBtn = document.getElementById('reset-btn');
        const targetDisplay = document.getElementById('target-display');
        const motivationText = document.getElementById('motivation-text');
        
        // 初始化
        function init() {
            // 设置日期输入的最小值为今天
            const today = new Date();
            targetDateInput.min = formatDate(today);
            
            // 设置默认日期为下一个周五
            setNextFriday();
            
            // 添加事件监听器
            targetDateInput.addEventListener('change', validateAndUpdateTarget);
            targetTimeInput.addEventListener('change', validateAndUpdateTarget);
            fridayBtn.addEventListener('click', setNextFriday);
            todayBtn.addEventListener('click', setToday);
            resetBtn.addEventListener('click', resetCountdown);
            
            // 开始倒计时
            updateCountdown();
            setInterval(updateCountdown, 1000);
        }
        
        // 验证并更新目标时间
        function validateAndUpdateTarget() {
            if (!targetDateInput.value) {
                return;
            }
            
            const selectedDate = new Date(targetDateInput.value);
            const today = new Date();
            today.setHours(0, 0, 0, 0);
            
            // 如果选择的日期是今天
            if (selectedDate.getTime() === today.getTime()) {
                const now = new Date();
                const selectedTime = targetTimeInput.value.split(':');
                const selectedHours = parseInt(selectedTime[0]);
                const selectedMinutes = parseInt(selectedTime[1]);
                
                // 如果选择的时间早于当前时间
                if (selectedHours < now.getHours() || 
                   (selectedHours === now.getHours() && selectedMinutes <= now.getMinutes())) {
                    // 设置为当前时间+30分钟
                    const newTime = new Date(now);
                    newTime.setMinutes(now.getMinutes() + 30);
                    targetTimeInput.value = formatTime(newTime);
                    
                    // 显示提示
                    motivationText.textContent = "时间已调整为当前时间后30分钟";
                    setTimeout(() => {
                        motivationText.textContent = "请设置目标时间开始倒计时";
                    }, 3000);
                }
            }
            
            updateTargetDateTime();
        }
        
        // 设置下一个周五
        function setNextFriday() {
            const now = new Date();
            const currentDay = now.getDay(); // 0是周日，5是周五
            let daysUntilFriday = 5 - currentDay;
            
            if (currentDay > 5 || (currentDay === 5 && now.getHours() >= 18)) {
                daysUntilFriday += 7;
            }
            
            const nextFriday = new Date(now);
            nextFriday.setDate(now.getDate() + daysUntilFriday);
            
            // 设置日期输入
            targetDateInput.value = formatDate(nextFriday);
            targetTimeInput.value = "18:00";
            
            updateTargetDateTime();
        }
        
        // 设置今天
        function setToday() {
            const now = new Date();
            
            // 设置日期输入
            targetDateInput.value = formatDate(now);
            
            // 如果当前时间已经超过18:00，设置为明天
            if (now.getHours() >= 18) {
                const tomorrow = new Date(now);
                tomorrow.setDate(now.getDate() + 1);
                targetDateInput.value = formatDate(tomorrow);
            }
            
            targetTimeInput.value = "18:00";
            
            updateTargetDateTime();
        }
        
        // 重置倒计时
        function resetCountdown() {
            targetDateInput.value = "";
            targetTimeInput.value = "18:00";
            targetDateTime = null;
            targetDisplay.textContent = "未设置";
            motivationText.textContent = "请设置目标时间开始倒计时";
            
            // 重置倒计时显示
            document.getElementById('hours').textContent = '00';
            document.getElementById('minutes').textContent = '00';
            document.getElementById('seconds').textContent = '00';
        }
        
        // 更新目标时间
        function updateTargetDateTime() {
            if (!targetDateInput.value) {
                targetDateTime = null;
                targetDisplay.textContent = "未设置";
                return;
            }
            
            const date = new Date(targetDateInput.value);
            const timeParts = targetTimeInput.value.split(':');
            
            if (timeParts.length === 2) {
                date.setHours(parseInt(timeParts[0]), parseInt(timeParts[1]), 0, 0);
                targetDateTime = date;
                
                // 更新显示
                targetDisplay.textContent = formatDateTime(targetDateTime);
                
                // 更新励志语句
                const randomIndex = Math.floor(Math.random() * motivations.length);
                motivationText.textContent = motivations[randomIndex];
            }
        }
        
        // 更新倒计时
        function updateCountdown() {
            if (!targetDateTime) {
                return;
            }
            
            const now = new Date();
            const timeDiff = targetDateTime - now;
            
            // 如果目标时间已过
            if (timeDiff <= 0) {
                document.getElementById('hours').textContent = '00';
                document.getElementById('minutes').textContent = '00';
                document.getElementById('seconds').textContent = '00';
                motivationText.textContent = "目标时间已到！";
                return;
            }
            
            // 计算总小时、分钟、秒（不显示天数）
            const totalHours = Math.floor(timeDiff / (1000 * 60 * 60));
            const minutes = Math.floor((timeDiff % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((timeDiff % (1000 * 60)) / 1000);
            
            // 更新倒计时显示
            document.getElementById('hours').textContent = totalHours.toString().padStart(2, '0');
            document.getElementById('minutes').textContent = minutes.toString().padStart(2, '0');
            document.getElementById('seconds').textContent = seconds.toString().padStart(2, '0');
            
            // 随机更新励志语句
            if (seconds % 30 === 0) {
                const randomIndex = Math.floor(Math.random() * motivations.length);
                motivationText.textContent = motivations[randomIndex];
            }
            
            // 更新周进度
            updateWeekProgress(now);
        }
        
        // 更新周进度
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
        
        // 工具函数：格式化日期为 YYYY-MM-DD
        function formatDate(date) {
            const year = date.getFullYear();
            const month = String(date.getMonth() + 1).padStart(2, '0');
            const day = String(date.getDate()).padStart(2, '0');
            return `${year}-${month}-${day}`;
        }
        
        // 工具函数：格式化时间为 HH:MM
        function formatTime(date) {
            const hours = String(date.getHours()).padStart(2, '0');
            const minutes = String(date.getMinutes()).padStart(2, '0');
            return `${hours}:${minutes}`;
        }
        
        // 工具函数：格式化日期时间为可读字符串
        function formatDateTime(date) {
            const options = { 
                year: 'numeric', 
                month: 'long', 
                day: 'numeric',
                hour: '2-digit',
                minute: '2-digit'
            };
            return date.toLocaleDateString('zh-CN', options);
        }
        
        // 初始化应用
        init();
    </script>
</body>
</html>

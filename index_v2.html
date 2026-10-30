<!DOCTYPE html>
<html lang="zh-Hant">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">
    <title>重整睡眠之旅 - 智慧活力習慣達成率版</title>
    <!-- 使用標準 link 載入 Noto Sans 字體 -->
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght=400;500;700;900&display=swap">
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://unpkg.com/react@18/umd/react.production.min.js"></script>
    <script src="https://unpkg.com/react-dom@18/umd/react-dom.production.min.js"></script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
    <!-- 鎖定 UMD 穩定版 Lucide 圖示 -->
    <script src="https://unpkg.com/lucide@0.469.0/dist/umd/lucide.min.js"></script>
    
    <script>
        // 註冊自訂 Babel 預設，強制使用 classic 模式，防範 React 18 /jsx-runtime 編譯錯誤
        window.Babel.registerPreset("custom-react", {
            presets: [
                [window.Babel.availablePresets["react"], { runtime: "classic" }]
            ]
        });
    </script>
    
    <style>
        body {
            font-family: 'Noto Sans TC', sans-serif;
            background-color: #f8fafc;
            user-select: none;
            -webkit-tap-highlight-color: transparent;
        }

        .soft-title-shadow {
            color: #1e293b;
            text-shadow: 0 4px 8px rgba(0, 0, 0, 0.06), 0 1px 3px rgba(0, 0, 0, 0.1);
        }

        .soft-subtitle-shadow {
            color: #64748b;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.04);
            letter-spacing: 0.025em;
        }

        .no-scrollbar::-webkit-scrollbar { display: none; }
        .no-scrollbar { -ms-overflow-style: none; scrollbar-width: none; }

        .active-scale { transition: transform 0.2s cubic-bezier(0.175, 0.885, 0.32, 1.275); }
        .active-scale:active { transform: scale(0.94); }

        @keyframes shine {
            from { transform: translateX(-100%) rotate(45deg); }
            to { transform: translateX(200%) rotate(45deg); }
        }
        .btn-shine {
            position: relative;
            overflow: hidden;
        }
        .btn-shine::after {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: rgba(255, 255, 255, 0.22);
            transform: rotate(45deg);
            animation: shine 3s infinite;
        }

        @keyframes fadeInScale {
            from { opacity: 0; transform: translateY(12px) scale(0.97); }
            to { opacity: 1; transform: translateY(0) scale(1); }
        }
        .animate-page { animation: fadeInScale 0.35s cubic-bezier(0.16, 1, 0.3, 1) forwards; }

        .progress-bar {
            transition: width 0.7s cubic-bezier(0.34, 1.56, 0.64, 1);
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-8px); }
        }
        .float-icon { animation: float 3s ease-in-out infinite; }

        @keyframes popIn {
            0% { transform: scale(0.85); opacity: 0; }
            100% { transform: scale(1); opacity: 1; }
        }
        .animate-pop { animation: popIn 0.3s cubic-bezier(0.175, 0.885, 0.32, 1.27) forwards; }

        @keyframes celebrateSpark {
            0%, 100% { transform: scale(1) rotate(0deg); opacity: 0.9; }
            50% { transform: scale(1.12) rotate(8deg); opacity: 1; }
        }
        .animate-celebrate { animation: celebrateSpark 2.5s infinite ease-in-out; }

        @keyframes burstConfetti {
            0% {
                transform: translate(0, 0) scale(0) rotate(0deg);
                opacity: 0;
            }
            15% {
                opacity: 1;
                transform: translate(0, -10px) scale(1.2) rotate(45deg);
            }
            100% {
                transform: translate(var(--tx), var(--ty)) scale(0.5) rotate(var(--rot));
                opacity: 0;
            }
        }
        .confetti-burst {
            position: absolute;
            animation: burstConfetti 2s cubic-bezier(0.1, 0.8, 0.3, 1) forwards;
            pointer-events: none;
            z-index: 150;
        }

        .overlay-blur {
            background: rgba(15, 23, 42, 0.75);
            backdrop-filter: blur(8px);
        }
    </style>
</head>
<body class="overflow-x-hidden pb-10">
    <div id="root"></div>

    <script type="text/babel" data-presets="custom-react">
        const { useState, useEffect, useMemo, useRef } = React;

        // 通用 Lucide 圖示封裝元件
        const Icon = ({ name, className = "w-5 h-5", size = 24 }) => {
            return <i data-lucide={name} className={className} style={{ width: size, height: size }}></i>;
        };

        // 療癒手繪風 - 小睡雲 (Sleeping Cloud)
        const SleepingCloudSVG = ({ className = "w-28 h-28 float-icon" }) => (
            <svg viewBox="0 0 100 100" className={className}>
                <path d="M25,65 a15,15 0 0,1 0,-25 a18,18 0 0,1 36,-5 a16,16 0 0,1 22,10 a15,15 0 0,1 -4,28 z" fill="#e0e7ff" stroke="#6366f1" strokeWidth="3.5" strokeLinejoin="round" />
                <path d="M36,54 q3,4 6,0" fill="none" stroke="#4338ca" strokeWidth="3" strokeLinecap="round" />
                <path d="M52,54 q3,4 6,0" fill="none" stroke="#4338ca" strokeWidth="3" strokeLinecap="round" />
                <circle cx="32" cy="58" r="4" fill="#fda4af" opacity="0.8" />
                <circle cx="62" cy="58" r="4" fill="#fda4af" opacity="0.8" />
                <path d="M43,36 q-10,-12 -20,-3 q0,10 13,8 z" fill="#818cf8" stroke="#4338ca" strokeWidth="2.5" />
                <circle cx="21" cy="31" r="3.5" fill="#ffffff" stroke="#4338ca" strokeWidth="2" />
                <polygon points="76,28 78,33 83,33 79,36 81,41 76,38 72,41 74,36 70,33 75,33" fill="#fef08a" />
            </svg>
        );

        // 活力手繪風 - 能量小星星 (Smiling Star)
        const GlowingStarSVG = ({ className = "w-28 h-28 animate-celebrate" }) => (
            <svg viewBox="0 0 100 100" className={className}>
                <polygon points="50,6 63,35 95,35 69,55 79,88 50,68 21,88 31,55 5,35 37,35" fill="#fef08a" stroke="#eab308" strokeWidth="3.5" strokeLinejoin="round" />
                <circle cx="39" cy="46" r="3" fill="#854d0e" />
                <circle cx="61" cy="46" r="3" fill="#854d0e" />
                <circle cx="34" cy="51" r="3" fill="#fca5a5" />
                <circle cx="66" cy="51" r="3" fill="#fca5a5" />
                <path d="M45,54 q5,5 10,0" fill="none" stroke="#854d0e" strokeWidth="3" strokeLinecap="round" />
                <path d="M12,12 L18,18 M88,12 L82,18" stroke="#f59e0b" strokeWidth="3" strokeLinecap="round" />
            </svg>
        );

        // 立體大獎盃 SVG
        const TrophySVG = ({ className = "w-20 h-20" }) => (
            <svg viewBox="0 0 100 100" className={className}>
                <ellipse cx="50" cy="85" rx="26" ry="5" fill="#e2e8f0" />
                <path d="M30,80 L70,80 L65,85 L35,85 Z" fill="#64748b" />
                <rect x="42" y="68" width="16" height="12" fill="#475569" rx="2" />
                <path d="M40,68 L60,68 L58,72 L42,72 Z" fill="#334155" />
                <path d="M46,50 L54,50 L54,68 L46,68 Z" fill="#d97706" />
                <path d="M25,23 C25,48 40,52 50,52 C60,52 75,48 75,23 L25,23 Z" fill="#f59e0b" stroke="#d97706" strokeWidth="3" strokeLinejoin="round" />
                <path d="M32,23 C32,43 42,46 50,46 C58,46 68,43 68,23 L32,23 Z" fill="#fbbf24" />
                <path d="M25,28 C12,28 12,43 25,43" fill="none" stroke="#d97706" strokeWidth="3.5" strokeLinecap="round" />
                <path d="M75,28 C88,28 88,43 75,43" fill="none" stroke="#d97706" strokeWidth="3.5" strokeLinecap="round" />
                <polygon points="50,28 53,34 60,35 55,40 56,46 50,43 44,46 45,40 40,35 47,34" fill="#ffffff" />
            </svg>
        );

        const TASK_THEMES = {
            '固定時間起床': { color: 'amber', icon: 'alarm-clock', bg: 'bg-amber-50', text: 'text-amber-600', ring: 'ring-amber-100', defaultAlarm: '07:30' },
            '曬日光 (出外曬太陽30-60 分鐘)': { color: 'orange', icon: 'sun', bg: 'bg-orange-50', text: 'text-orange-600', ring: 'ring-orange-100', defaultAlarm: '08:30' },
            '出外做運動 (45-60 分鐘，如：慢跑、快走)': { color: 'emerald', icon: 'bike', bg: 'bg-emerald-50', text: 'text-emerald-600', ring: 'ring-emerald-100', defaultAlarm: '17:00' },
            '避免日間躺在睡床上': { color: 'amber', icon: 'sofa', bg: 'bg-amber-50', text: 'text-amber-600', ring: 'ring-amber-100', defaultAlarm: '13:00' },
            '聽放鬆音樂 (30-45分鐘)': { color: 'indigo', icon: 'music', bg: 'bg-indigo-50', text: 'text-indigo-600', ring: 'ring-indigo-100', defaultAlarm: '21:30' },
            '呼吸練習 (10-15分鐘)': { color: 'sky', icon: 'wind', bg: 'bg-sky-50', text: 'text-sky-600', ring: 'ring-sky-100', defaultAlarm: '22:00' },
            '熱敷 (眼/肩/頸/背)': { color: 'rose', icon: 'thermometer-sun', bg: 'bg-rose-50', text: 'text-rose-600', ring: 'ring-rose-100', defaultAlarm: '22:15' },
            '拉筋伸展運動 (15-20 分鐘)': { color: 'violet', icon: 'flower', bg: 'bg-violet-50', text: 'text-violet-600', ring: 'ring-violet-100', defaultAlarm: '21:45' },
            '減少/避免在中午後飲用有咖啡因飲品 (咖啡、奶茶、茶、可樂)': { color: 'cyan', icon: 'coffee', bg: 'bg-cyan-50', text: 'text-cyan-600', ring: 'ring-cyan-100', defaultAlarm: '12:00' },
            '睡前至少30分鐘停止使用電子產品，如：手機、電視、平板': { color: 'cyan', icon: 'smartphone', bg: 'bg-cyan-50', text: 'text-cyan-600', ring: 'ring-cyan-100', defaultAlarm: '22:30' },
            '避免在床上做和睡眠沒有關係的事，如：看電視/手機、進食': { color: 'cyan', icon: 'bed', bg: 'bg-cyan-50', text: 'text-cyan-600', ring: 'ring-cyan-100', defaultAlarm: '21:00' },
            '等待有睡意才上床': { color: 'cyan', icon: 'cloud-moon', bg: 'bg-cyan-50', text: 'text-cyan-600', ring: 'ring-cyan-100', defaultAlarm: '23:00' },
            '移除臥室內的計時裝置，如：鬧鐘、手提電話': { color: 'cyan', icon: 'watch', bg: 'bg-cyan-50', text: 'text-cyan-600', ring: 'ring-cyan-100', defaultAlarm: '22:45' }
        };

        const CATEGORIES = [
            {
                id: 'daytime',
                title: '日間活動習慣',
                icon: 'sun',
                color: 'amber',
                bgClass: 'bg-amber-50/60',
                borderClass: 'border-amber-200',
                items: [
                    { name: '固定時間起床', hint: '即使假日也建議維持相同作息' },
                    { name: '曬日光 (出外曬太陽30-60 分鐘)', hint: '光照有助於調節生理時鐘' },
                    { name: '出外做運動 (45-60 分鐘，如：慢跑、快走)', hint: '適度運動能幫助晚間深層睡眠' },
                    { name: '避免日間躺在睡床上', hint: '床應僅用於睡眠，日間活動應在沙發或桌椅進行' }
                ]
            },
            {
                id: 'hygiene',
                title: '睡眠衛生習慣',
                icon: 'shield-check',
                color: 'cyan',
                bgClass: 'bg-cyan-50/70',
                borderClass: 'border-cyan-200',
                items: [
                    { name: '減少/避免在中午後飲用有咖啡因飲品 (咖啡、奶茶、茶、可樂)', hint: '咖啡因會干擾大腦化學機制' },
                    { name: '睡前至少30分鐘停止使用電子產品，如：手機、電視、平板', hint: '藍光會顯著抑制褪黑激素分泌' },
                    { name: '避免在床上做和睡眠沒有關係的事，如：看電視/手機、進食', hint: '強化大腦對床與睡眠的連結' },
                    { name: '等待有睡意才上床', hint: '避免在床上清醒掙扎而產生焦慮' },
                    { name: '移除臥室內的計時裝置，如：鬧鐘、手提電話', hint: '減少半夜看時間產生的壓力' }
                ]
            },
            {
                id: 'rituals',
                title: '睡前放鬆儀式',
                icon: 'moon',
                color: 'indigo',
                bgClass: 'bg-indigo-50/60',
                borderClass: 'border-indigo-200',
                items: [
                    { name: '聽放鬆音樂 (30-45分鐘)', hint: '讓節奏慢下來，準備睡眠訊號' },
                    { name: '呼吸練習 (10-15分鐘)', hint: '專注於深緩呼吸，放鬆神經系統' },
                    { name: '熱敷 (眼/肩/頸/背)', hint: '提升局部循環並降低核心溫度感' },
                    { name: '拉筋伸展運動 (15-20 分鐘)', hint: '輕柔舒展身體，緩解肌肉緊繃，放鬆並幫助入睡' }
                ]
            }
        ];

        const DURATION_THEMES = {
            7: { 
                name: 'emerald', 
                cardDone: 'bg-emerald-50/70 border-emerald-200 text-slate-700', 
                btnDone: 'bg-emerald-500 border-emerald-500 text-white shadow-md shadow-emerald-100',
                progressFill: 'bg-emerald-400',
                barFill: 'bg-emerald-500',
                textAccent: 'text-emerald-600'
            },
            14: { 
                name: 'amber', 
                cardDone: 'bg-amber-50/70 border-amber-200 text-slate-700', 
                btnDone: 'bg-amber-500 border-amber-500 text-white shadow-md shadow-amber-100',
                progressFill: 'bg-amber-400',
                barFill: 'bg-amber-500',
                textAccent: 'text-amber-600'
            },
            21: { 
                name: 'purple', 
                cardDone: 'bg-purple-50/70 border-purple-200 text-slate-700', 
                btnDone: 'bg-purple-600 border-purple-600 text-white shadow-md shadow-purple-100',
                progressFill: 'bg-purple-400',
                barFill: 'bg-purple-600',
                textAccent: 'text-purple-600'
            }
        };

        const Footer = () => (
            <div className="w-full flex items-center justify-center gap-1.5 pt-2 pb-0.5 text-slate-400 text-xs font-bold tracking-widest">
                <Icon name="heart" size={14} className="text-red-400 fill-red-400/30" />
                <span>QEH OT</span>
            </div>
        );

        // 日期格式化為 DD/MM/YYYY (日/月/年)
        const formatDateDDMMYYYY = (isoDateStr) => {
            if (!isoDateStr) return '';
            const parts = isoDateStr.split('-');
            if (parts.length !== 3) return isoDateStr;
            return `${parts[2]}/${parts[1]}/${parts[0]}`;
        };

        // 計算指定年月之月曆天數陣列 (確保跨平台/跨瀏覽器/iFrame皆能穩定彈出選擇)
        const getCalendarDays = (year, month) => {
            const firstDay = new Date(year, month, 1).getDay(); // 0 = 星期日
            const daysInMonth = new Date(year, month + 1, 0).getDate();
            const daysInPrevMonth = new Date(year, month, 0).getDate();

            const days = [];

            // 上個月補齊天數
            for (let i = firstDay - 1; i >= 0; i--) {
                const d = daysInPrevMonth - i;
                const prevMonth = month === 0 ? 11 : month - 1;
                const prevYear = month === 0 ? year - 1 : year;
                const dateStr = `${prevYear}-${String(prevMonth + 1).padStart(2, '0')}-${String(d).padStart(2, '0')}`;
                days.push({ day: d, isCurrentMonth: false, dateStr });
            }

            // 當月天數
            for (let d = 1; d <= daysInMonth; d++) {
                const dateStr = `${year}-${String(month + 1).padStart(2, '0')}-${String(d).padStart(2, '0')}`;
                days.push({ day: d, isCurrentMonth: true, dateStr });
            }

            // 下個月補齊至 35 或 42 格
            const totalCells = days.length > 35 ? 42 : 35;
            const remaining = totalCells - days.length;
            for (let d = 1; d <= remaining; d++) {
                const nextMonth = month === 11 ? 0 : month + 1;
                const nextYear = month === 11 ? year + 1 : year;
                const dateStr = `${nextYear}-${String(nextMonth + 1).padStart(2, '0')}-${String(d).padStart(2, '0')}`;
                days.push({ day: d, isCurrentMonth: false, dateStr });
            }

            return days;
        };

        function App() {
            const [appMode, setAppMode] = useState('setup'); // 'setup' | 'tracking'
            const [setupStep, setSetupStep] = useState(1);
            const [planDuration, setPlanDuration] = useState(7);
            const [startDate, setStartDate] = useState(new Date().toISOString().split('T')[0]);
            const [selectedTasks, setSelectedTasks] = useState(new Set());
            const [dailyLogs, setDailyLogs] = useState({});
            const [taskAlarms, setTaskAlarms] = useState({});
            const [trackingStartedAt, setTrackingStartedAt] = useState(null);

            // 自訂月曆彈窗 State
            const [showDatePickerModal, setShowDatePickerModal] = useState(false);
            const initialDate = new Date(startDate || Date.now());
            const [calYear, setCalYear] = useState(initialDate.getFullYear());
            const [calMonth, setCalMonth] = useState(initialDate.getMonth());

            const [showSuccessToast, setShowSuccessToast] = useState(false);
            const [activeRitual, setActiveRitual] = useState(null);
            const [alarmSettingTask, setAlarmSettingTask] = useState(null);
            const [triggeredAlarm, setTriggeredAlarm] = useState(null);
            const [showResetConfirm, setShowResetConfirm] = useState(false);
            const [showStatsModal, setShowStatsModal] = useState(false);
            const [notificationPermission, setNotificationPermission] = useState('default');

            const [showSingleEncouragement, setShowSingleEncouragement] = useState(false);
            const [mascotType, setMascotType] = useState('cloud');
            const [confettiArray, setConfettiArray] = useState([]);

            // 讀取 localStorage
            useEffect(() => {
                try {
                    const saved = localStorage.getItem('SleepApp_V6_CompletionRate');
                    if (saved) {
                        const data = JSON.parse(saved);
                        if (data.appMode) setAppMode(data.appMode);
                        if (data.planDuration) setPlanDuration(data.planDuration);
                        if (data.startDate) {
                            setStartDate(data.startDate);
                            const d = new Date(data.startDate);
                            if (!isNaN(d.getTime())) {
                                setCalYear(d.getFullYear());
                                setCalMonth(d.getMonth());
                            }
                        }
                        if (data.selectedTasks) setSelectedTasks(new Set(data.selectedTasks));
                        if (data.dailyLogs) setDailyLogs(data.dailyLogs);
                        if (data.taskAlarms) setTaskAlarms(data.taskAlarms);
                        if (data.trackingStartedAt) setTrackingStartedAt(data.trackingStartedAt);
                        if (data.selectedTasks && data.selectedTasks.length > 0 && data.appMode === 'setup') {
                            setSetupStep(2);
                        }
                    }
                } catch (e) { console.warn("無法讀取 localStorage。"); }

                if ('Notification' in window) {
                    setNotificationPermission(Notification.permission);
                }
            }, []);

            // Lucide 圖示 DOM 轉換重繪
            useEffect(() => {
                if (window.lucide) window.lucide.createIcons();
            });

            // 儲存至 localStorage
            useEffect(() => {
                try {
                    localStorage.setItem('SleepApp_V6_CompletionRate', JSON.stringify({
                        appMode, planDuration, startDate, dailyLogs, taskAlarms, trackingStartedAt,
                        selectedTasks: Array.from(selectedTasks)
                    }));
                } catch (e) {}
            }, [appMode, planDuration, startDate, selectedTasks, dailyLogs, taskAlarms, trackingStartedAt]);

            // 核心邏輯：計算習慣達成率數據
            const stats = useMemo(() => {
                const today = new Date().toISOString().split('T')[0];
                const sDate = new Date(startDate);
                sDate.setHours(0,0,0,0);
                const cDate = new Date(today);
                cDate.setHours(0,0,0,0);
                
                // 計算計畫啟動天數 (至少第 1 天，上限為計畫總天數)
                const diffTime = cDate - sDate;
                const rawDays = Math.floor(diffTime / (1000 * 60 * 60 * 24)) + 1;
                const elapsedDays = Math.min(planDuration, Math.max(1, rawDays));

                const taskList = Array.from(selectedTasks);
                const totalPossibleCompletions = elapsedDays * taskList.length;

                let totalActualCompletions = 0;
                const perTaskStats = {};

                taskList.forEach(task => {
                    perTaskStats[task] = 0;
                });

                // 統計計畫開始至今的每一天完成情況
                for (let i = 0; i < elapsedDays; i++) {
                    const tempDate = new Date(sDate);
                    tempDate.setDate(tempDate.getDate() + i);
                    const dateStr = tempDate.toISOString().split('T')[0];
                    const dayLog = dailyLogs[dateStr] || [];

                    taskList.forEach(task => {
                        if (dayLog.includes(task)) {
                            totalActualCompletions += 1;
                            perTaskStats[task] = (perTaskStats[task] || 0) + 1;
                        }
                    });
                }

                // 整體習慣達成率
                const overallRate = totalPossibleCompletions > 0 
                    ? Math.round((totalActualCompletions / totalPossibleCompletions) * 100) 
                    : 0;

                // 今日習慣達成率
                const todayLog = dailyLogs[today] || [];
                const todayCompletedCount = taskList.filter(t => todayLog.includes(t)).length;
                const todayRate = taskList.length > 0 
                    ? Math.round((todayCompletedCount / taskList.length) * 100) 
                    : 0;

                // 計算連續堅持天數 (Streak)
                let streak = 0;
                for (let i = rawDays - 1; i >= 0; i--) {
                    const tempDate = new Date(sDate);
                    tempDate.setDate(tempDate.getDate() + i);
                    const dateStr = tempDate.toISOString().split('T')[0];
                    const dayLog = dailyLogs[dateStr] || [];
                    if (dayLog.length > 0) {
                        streak += 1;
                    } else if (i < rawDays - 1) { // 如果今天還沒填算0，但若昨天斷掉就停止
                        break;
                    }
                }

                return {
                    elapsedDays,
                    totalPossibleCompletions,
                    totalActualCompletions,
                    overallRate,
                    todayRate,
                    todayCompletedCount,
                    totalSelectedCount: taskList.length,
                    perTaskStats,
                    streak
                };
            }, [startDate, planDuration, selectedTasks, dailyLogs]);

            // 系統通知與鬧鐘邏輯
            const triggerSystemNotification = (taskName) => {
                if ('Notification' in window && Notification.permission === 'granted') {
                    try {
                        const notify = new Notification("重整睡眠之旅 ⏰ 任務提醒", {
                            body: `現在該執行「${taskName}」囉！點擊立刻進行睡眠管理。`,
                            icon: "https://placehold.co/128x128/6366f1/ffffff?text=Sleep",
                            requireInteraction: true
                        });

                        notify.onclick = () => {
                            window.focus();
                            setAppMode('tracking');
                            setTriggeredAlarm(null);
                            const foundTask = CATEGORIES.flatMap(c => c.items).find(i => i.name === taskName);
                            if (foundTask) setActiveRitual(foundTask);
                            notify.close();
                        };
                    } catch (err) { console.warn(err); }
                }
            };

            useEffect(() => {
                const timer = setInterval(() => {
                    if (appMode !== 'tracking') return;
                    const now = new Date();
                    const currentTime = `${String(now.getHours()).padStart(2, '0')}:${String(now.getMinutes()).padStart(2, '0')}`;
                    const todayStr = now.toISOString().split('T')[0];
                    const todayDone = dailyLogs[todayStr] || [];

                    Object.entries(taskAlarms).forEach(([task, time]) => {
                        if (time === currentTime && !todayDone.includes(task) && triggeredAlarm !== task) {
                            setTriggeredAlarm(task);
                            triggerSystemNotification(task);
                        }
                    });
                }, 10000);
                return () => clearInterval(timer);
            }, [taskAlarms, dailyLogs, appMode, triggeredAlarm]);

            const generateConfetti = () => {
                const colors = ['#f59e0b', '#10b981', '#3b82f6', '#ec4899', '#8b5cf6', '#34d399', '#fcd34d'];
                const items = [];
                for (let i = 0; i < 35; i++) {
                    const angle = (Math.random() * 140 + 20) * (Math.PI / 180);
                    const distance = Math.random() * 130 + 50;
                    const tx = `${Math.cos(angle) * distance}px`;
                    const ty = `-${Math.sin(angle) * distance}px`;
                    const rot = `${Math.random() * 360 + 360}deg`;

                    items.push({
                        id: i, tx, ty, rot,
                        delay: `${Math.random() * 0.3}s`,
                        color: colors[Math.floor(Math.random() * colors.length)],
                        size: `${Math.random() * 8 + 8}px`,
                        shape: Math.random() > 0.5 ? 'rounded-full' : 'rotate-45'
                    });
                }
                setConfettiArray(items);
            };

            const todayStr = new Date().toISOString().split('T')[0];

            const handleStartTracking = () => {
                const updatedAlarms = { ...taskAlarms };
                selectedTasks.forEach(task => {
                    if (!updatedAlarms[task]) {
                        updatedAlarms[task] = TASK_THEMES[task]?.defaultAlarm || "08:00";
                    }
                });
                setTaskAlarms(updatedAlarms);
                setTrackingStartedAt(Date.now());
                setAppMode('tracking');
                if ('Notification' in window) Notification.requestPermission();
            };

            const toggleTask = (taskName) => {
                const dayLog = dailyLogs[todayStr] || [];
                const isCompleting = !dayLog.includes(taskName);
                if (isCompleting) {
                    const foundTask = CATEGORIES.flatMap(c => c.items).find(i => i.name === taskName);
                    setActiveRitual(foundTask);
                } else {
                    let newLog = dayLog.filter(t => t !== taskName);
                    setDailyLogs({ ...dailyLogs, [todayStr]: newLog });
                }
            };

            const confirmRitual = () => {
                if (!activeRitual) return;
                const taskName = activeRitual.name;
                const dayLog = dailyLogs[todayStr] || [];
                let newLog = [...dayLog, taskName];
                
                setMascotType(Math.random() > 0.5 ? 'cloud' : 'star');

                setDailyLogs({ ...dailyLogs, [todayStr]: newLog });
                setActiveRitual(null);
                setTriggeredAlarm(null);

                if (newLog.length === selectedTasks.size) {
                    generateConfetti();
                    setShowSuccessToast(true);
                } else {
                    setShowSingleEncouragement(true);
                }
            };

            const executeReset = () => {
                setAppMode('setup');
                setSetupStep(1);
                setDailyLogs({});
                setSelectedTasks(new Set());
                setTaskAlarms({});
                setTrackingStartedAt(null);
                const tDate = new Date().toISOString().split('T')[0];
                setStartDate(tDate);
                const d = new Date();
                setCalYear(d.getFullYear());
                setCalMonth(d.getMonth());
                setShowResetConfirm(false);
            };

            const SetupView = () => (
                <div className="animate-page flex flex-col min-h-screen max-w-md mx-auto p-5">
                    <header className="mt-8 mb-6 text-center">
                        <div className="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-indigo-50 text-indigo-600 text-xs font-bold mb-2">
                            <Icon name="sparkles" size={14} /> 建立你的優質睡眠習慣
                        </div>
                        <h1 className="text-4xl font-black tracking-tight text-slate-800">重整睡眠之旅</h1>
                        <p className="font-bold mt-1 text-base text-slate-500">睡眠管理行動計劃</p>
                    </header>

                    {setupStep === 1 ? (
                        <div className="space-y-5 flex-1 pb-36">
                            <div className="text-center">
                                <span className="text-xs font-extrabold text-indigo-600 bg-indigo-100/70 px-4 py-1.5 rounded-full">
                                    步驟 1：選擇挑戰習慣 (可多選)
                                </span>
                            </div>
                            
                            {CATEGORIES.map(cat => (
                                <section key={cat.id} className={`${cat.bgClass} ${cat.borderClass} border-2 rounded-3xl p-4 space-y-3`}>
                                    <div className="flex items-center gap-2">
                                        <div className={`p-2 rounded-xl bg-white shadow-sm text-${cat.color}-600`}>
                                            <Icon name={cat.icon} size={18} />
                                        </div>
                                        <h3 className="text-base font-bold text-slate-800">{cat.title}</h3>
                                    </div>
                                    <div className="space-y-2">
                                        {cat.items.map(item => {
                                            const isSelected = selectedTasks.has(item.name);
                                            return (
                                                <div 
                                                    key={item.name}
                                                    onClick={() => {
                                                        const next = new Set(selectedTasks);
                                                        if(isSelected) next.delete(item.name); else next.add(item.name);
                                                        setSelectedTasks(next);
                                                    }}
                                                    className={`p-3.5 rounded-2xl border-2 transition-all active-scale cursor-pointer flex items-center justify-between ${
                                                        isSelected ? 'border-indigo-600 bg-white shadow-md' : 'border-slate-200/60 bg-white/60 hover:bg-white'
                                                    }`}
                                                >
                                                    <div className="flex-1 pr-2">
                                                        <p className="text-sm font-bold text-slate-800">{item.name}</p>
                                                        <p className="text-[11px] text-slate-500 mt-0.5">{item.hint}</p>
                                                    </div>
                                                    <div className={`w-6 h-6 rounded-full border-2 flex items-center justify-center transition-colors ${
                                                        isSelected ? 'bg-indigo-600 border-indigo-600 text-white' : 'border-slate-300'
                                                    }`}>
                                                        {isSelected && <Icon name="check" size={14} />}
                                                    </div>
                                                </div>
                                            );
                                        })}
                                    </div>
                                </section>
                            ))}

                            <div className="fixed bottom-0 left-0 right-0 p-4 bg-white/90 backdrop-blur-md border-t border-slate-100 flex flex-col items-center justify-center max-w-md mx-auto z-40">
                                <button
                                    disabled={selectedTasks.size === 0}
                                    onClick={() => setSetupStep(2)}
                                    className={`w-full py-3.5 rounded-2xl font-black text-white shadow-lg transition-all active-scale flex items-center justify-center gap-2 ${
                                        selectedTasks.size > 0 ? 'bg-indigo-600 shadow-indigo-200 hover:bg-indigo-700' : 'bg-slate-300 cursor-not-allowed'
                                    }`}
                                >
                                    下一步：設定天數與開始日 ({selectedTasks.size})
                                    <Icon name="arrow-right" size={18} />
                                </button>
                                <Footer />
                            </div>
                        </div>
                    ) : (
                        <div className="space-y-6 flex-1 pb-36">
                            <div className="text-center">
                                <span className="text-xs font-extrabold text-indigo-600 bg-indigo-100/70 px-4 py-1.5 rounded-full">
                                    步驟 2：選擇挑戰週期
                                </span>
                            </div>

                            <div className="bg-white rounded-3xl p-5 border-2 border-slate-100 shadow-sm space-y-4">
                                <label className="block text-sm font-bold text-slate-700">挑戰總天數</label>
                                <div className="grid grid-cols-3 gap-3">
                                    {[
                                        { 
                                            days: 7, 
                                            title: '7', 
                                            subtitle: '7天挑戰', 
                                            active: 'bg-emerald-500 border-emerald-500 text-white shadow-md shadow-emerald-100 ring-2 ring-emerald-300', 
                                            inactive: 'bg-emerald-50/70 border-emerald-200 text-emerald-800 hover:bg-emerald-100/80' 
                                        },
                                        { 
                                            days: 14, 
                                            title: '14', 
                                            subtitle: '14天挑戰', 
                                            active: 'bg-amber-500 border-amber-500 text-white shadow-md shadow-amber-100 ring-2 ring-amber-300', 
                                            inactive: 'bg-amber-50/70 border-amber-200 text-amber-800 hover:bg-amber-100/80' 
                                        },
                                        { 
                                            days: 21, 
                                            title: '21', 
                                            subtitle: '21天挑戰', 
                                            active: 'bg-purple-600 border-purple-600 text-white shadow-md shadow-purple-100 ring-2 ring-purple-300', 
                                            inactive: 'bg-purple-50/70 border-purple-200 text-purple-800 hover:bg-purple-100/80' 
                                        }
                                    ].map(opt => {
                                        const isSelected = planDuration === opt.days;
                                        return (
                                            <button
                                                key={opt.days}
                                                onClick={() => setPlanDuration(opt.days)}
                                                className={`py-4 rounded-2xl border-2 font-black transition-all active-scale flex flex-col items-center justify-center ${
                                                    isSelected ? opt.active : opt.inactive
                                                }`}
                                            >
                                                <span className="text-2xl">{opt.days}</span>
                                                <span className="text-xs font-semibold">{opt.subtitle}</span>
                                            </button>
                                        );
                                    })}
                                </div>
                            </div>

                            {}
                            <div className="bg-white rounded-3xl p-5 border-2 border-slate-100 shadow-sm space-y-3">
                                <div className="flex items-center justify-between">
                                    <label className="block text-sm font-bold text-slate-700">開始日期</label>
                                </div>
                                
                                <div 
                                    onClick={() => {
                                        const d = new Date(startDate || Date.now());
                                        if (!isNaN(d.getTime())) {
                                            setCalYear(d.getFullYear());
                                            setCalMonth(d.getMonth());
                                        }
                                        setShowDatePickerModal(true);
                                    }}
                                    className="relative cursor-pointer group rounded-2xl border-2 border-indigo-100 hover:border-indigo-400 bg-indigo-50/30 p-3.5 flex items-center justify-between transition-all active-scale shadow-sm"
                                >
                                    <div className="flex items-center gap-3">
                                        <div className="p-2.5 rounded-xl bg-indigo-600 text-white shadow-md shadow-indigo-200">
                                            <Icon name="calendar-days" size={20} />
                                        </div>
                                        <div>
                                            <p className="text-xs font-semibold text-slate-400">目前選擇日期 (日/月/年)</p>
                                            <p className="text-lg font-black text-slate-800 tracking-wide">
                                                {formatDateDDMMYYYY(startDate)}
                                            </p>
                                        </div>
                                    </div>

                                    <div className="px-3.5 py-2 rounded-xl bg-indigo-600 text-white font-bold text-xs shadow-md shadow-indigo-100 hover:bg-indigo-700 transition-colors flex items-center gap-1.5">
                                        <Icon name="calendar-plus" size={15} />
                                        點擊開啟日曆
                                    </div>
                                </div>
                                <p className="text-[11px] text-slate-400 font-medium text-center pt-0.5">點擊上方區塊即可輕鬆彈出日曆面板進行日期選擇</p>
                            </div>

                            <div className="bg-indigo-50/70 rounded-3xl p-5 border-2 border-indigo-100 space-y-2">
                                <h4 className="text-sm font-bold text-indigo-900 flex items-center gap-2">
                                    <Icon name="check-circle-2" size={16} className="text-indigo-600" /> 已選擇的習慣項目 ({selectedTasks.size})
                                </h4>
                                <ul className="text-xs font-medium text-indigo-700 space-y-1 list-disc list-inside">
                                    {Array.from(selectedTasks).map(t => (
                                        <li key={t}>{t}</li>
                                    ))}
                                </ul>
                            </div>

                            <div className="fixed bottom-0 left-0 right-0 p-4 bg-white/90 backdrop-blur-md border-t border-slate-100 flex flex-col items-center justify-center max-w-md mx-auto z-40">
                                <div className="flex gap-3 w-full">
                                    <button
                                        onClick={() => setSetupStep(1)}
                                        className="px-5 py-3.5 rounded-2xl font-bold bg-slate-100 text-slate-600 hover:bg-slate-200 transition-colors"
                                    >
                                        上一步
                                    </button>
                                    <button
                                        onClick={handleStartTracking}
                                        className="flex-1 py-3.5 rounded-2xl font-black text-white bg-indigo-600 shadow-lg shadow-indigo-200 hover:bg-indigo-700 active-scale btn-shine flex items-center justify-center gap-2"
                                    >
                                        開啟我的睡眠之旅
                                        <Icon name="rocket" size={18} />
                                    </button>
                                </div>
                                <Footer />
                            </div>
                        </div>
                    )}
                </div>
            );

            const TrackingView = () => {
                const currentTheme = DURATION_THEMES[planDuration] || DURATION_THEMES[7];

                return (
                    <div className="animate-page flex flex-col min-h-screen max-w-md mx-auto p-4 space-y-4">
                        {/* 頂部標題與重置設定 */}
                        <div className="flex items-center justify-between pt-2 px-1">
                            <div>
                                <h2 className="text-3xl font-black text-slate-800 tracking-tight">重整睡眠之旅</h2>
                                <p className="text-xs font-bold text-slate-400">第 {stats.elapsedDays} / {planDuration} 天挑戰中</p>
                            </div>
                            <button
                                onClick={() => setShowResetConfirm(true)}
                                className="p-2.5 rounded-2xl bg-slate-100 text-slate-500 hover:bg-slate-200 active-scale"
                                title="重新設定計畫"
                            >
                                <Icon name="rotate-ccw" size={18} />
                            </button>
                        </div>

                        {/* 習慣達成率 Hero 儀表板 */}
                        <div className="bg-gradient-to-br from-indigo-600 via-indigo-700 to-purple-800 rounded-3xl p-5 text-white shadow-xl shadow-indigo-200 relative overflow-hidden">
                            <div className="absolute top-0 right-0 -mr-6 -mt-6 w-32 h-32 bg-white/10 rounded-full blur-2xl pointer-events-none"></div>

                            <div className="flex items-center justify-between mb-4">
                                <div className="flex items-center gap-2 bg-white/15 px-3 py-1 rounded-full backdrop-blur-md">
                                    <Icon name="activity" size={14} className="text-emerald-300" />
                                    <span className="text-xs font-bold tracking-wide text-indigo-100">睡眠習慣達成率</span>
                                </div>
                                <button 
                                    onClick={() => setShowStatsModal(true)}
                                    className="text-xs font-bold bg-white text-indigo-900 px-3 py-1 rounded-full shadow-sm hover:bg-indigo-50 active-scale flex items-center gap-1"
                                >
                                    <Icon name="bar-chart-2" size={13} />
                                    詳細報表
                                </button>
                            </div>

                            <div className="grid grid-cols-2 gap-3 items-center">
                                {/* 整體累積達成率 */}
                                <div className="bg-white/10 p-3.5 rounded-2xl border border-white/10 backdrop-blur-sm">
                                    <p className="text-[11px] font-medium text-indigo-200 mb-1">整體累積達成率</p>
                                    <div className="flex items-baseline gap-1">
                                        <span className="text-3xl font-black tracking-tight">{stats.overallRate}%</span>
                                    </div>
                                    <div className="w-full bg-white/20 h-1.5 rounded-full mt-2 overflow-hidden">
                                        <div 
                                            className={`${currentTheme.progressFill} h-full rounded-full transition-all duration-700`} 
                                            style={{ width: `${stats.overallRate}%` }}
                                        ></div>
                                    </div>
                                </div>

                                {/* 今日達成率 & Streak */}
                                <div className="bg-white/10 p-3.5 rounded-2xl border border-white/10 backdrop-blur-sm space-y-1">
                                    <p className="text-[11px] font-medium text-indigo-200">今日完成進度</p>
                                    <div className="flex items-baseline justify-between">
                                        <span className="text-2xl font-extrabold">{stats.todayCompletedCount}/{stats.totalSelectedCount}</span>
                                        <span className="text-xs font-bold text-amber-300 bg-amber-400/20 px-2 py-0.5 rounded-md border border-amber-300/30">
                                            {stats.todayRate}%
                                        </span>
                                    </div>
                                    <p className="text-[10px] text-indigo-200 flex items-center gap-1 mt-1">
                                        <Icon name="flame" size={12} className="text-orange-400 fill-orange-400" />
                                        連續打卡: <span className="font-bold text-white">{stats.streak} 天</span>
                                    </p>
                                </div>
                            </div>
                        </div>

                        {/* 今日習慣打卡清單 */}
                        <div className="space-y-3">
                            <div className="flex items-center justify-between px-1">
                                <h3 className="text-base font-bold text-slate-800 flex items-center gap-2">
                                    <Icon name="calendar-check" size={18} className="text-indigo-600" />
                                    今日挑戰習慣 ({formatDateDDMMYYYY(todayStr)})
                                </h3>
                                <span className="text-xs font-bold text-slate-400">
                                    完成 {stats.todayCompletedCount} / {stats.totalSelectedCount}
                                </span>
                            </div>

                            <div className="space-y-2.5">
                                {Array.from(selectedTasks).map(taskName => {
                                    const isDone = (dailyLogs[todayStr] || []).includes(taskName);
                                    const alarmTime = taskAlarms[taskName];

                                    return (
                                        <div 
                                            key={taskName}
                                            className={`p-4 rounded-3xl border-2 transition-all active-scale flex items-center justify-between ${
                                                isDone ? currentTheme.cardDone : 'bg-white border-slate-100 shadow-sm hover:border-slate-200'
                                            }`}
                                        >
                                            <div className="flex items-center gap-3.5 flex-1 pr-2">
                                                <button
                                                    onClick={() => toggleTask(taskName)}
                                                    className={`w-7 h-7 rounded-2xl border-2 flex items-center justify-center transition-all ${
                                                        isDone ? currentTheme.btnDone : 'border-slate-300 bg-slate-50'
                                                    }`}
                                                >
                                                    {isDone && <Icon name="check" size={16} />}
                                                </button>
                                                
                                                <div className="flex-1" onClick={() => toggleTask(taskName)}>
                                                    <p className={`text-sm font-bold ${isDone ? 'line-through text-slate-400' : 'text-slate-800'}`}>
                                                        {taskName}
                                                    </p>
                                                    {alarmTime && (
                                                        <span className="inline-flex items-center gap-1 text-[11px] font-semibold text-slate-400 mt-0.5">
                                                            <Icon name="clock" size={12} /> 提醒: {alarmTime}
                                                        </span>
                                                    )}
                                                </div>
                                            </div>

                                            {/* 鬧鐘設定按鈕 */}
                                            <button
                                                onClick={() => setAlarmSettingTask(taskName)}
                                                className="p-2 rounded-xl bg-slate-100/80 text-slate-500 hover:bg-slate-200 text-xs font-bold flex items-center gap-1"
                                                title="設定提醒時間"
                                            >
                                                <Icon name="bell" size={15} />
                                            </button>
                                        </div>
                                    );
                                })}
                            </div>
                        </div>

                        <Footer />
                    </div>
                );
            };

            const daysGrid = getCalendarDays(calYear, calMonth);
            const todayIso = new Date().toISOString().split('T')[0];

            const changeMonth = (offset) => {
                let newM = calMonth + offset;
                let newY = calYear;
                if (newM < 0) {
                    newM = 11;
                    newY -= 1;
                } else if (newM > 11) {
                    newM = 0;
                    newY += 1;
                }
                setCalMonth(newM);
                setCalYear(newY);
            };

            return (
                <div className="min-h-screen bg-slate-50 relative selection:bg-indigo-500 selection:text-white">
                    {appMode === 'setup' ? <SetupView /> : <TrackingView />}

                    {/* 📅 自訂互動式日曆選擇 Modal */}
                    {showDatePickerModal && (
                        <div className="fixed inset-0 z-50 overlay-blur flex items-center justify-center p-4 animate-pop">
                            <div className="bg-white rounded-3xl max-w-sm w-full p-5 shadow-2xl border border-slate-100 space-y-4">
                                <div className="flex items-center justify-between pb-2 border-b border-slate-100">
                                    <div className="flex items-center gap-2">
                                        <div className="p-2 bg-indigo-50 text-indigo-600 rounded-xl">
                                            <Icon name="calendar-days" size={20} />
                                        </div>
                                        <div>
                                            <h3 className="text-base font-black text-slate-800">選擇開始日期</h3>
                                            <p className="text-[11px] text-slate-400">目前選擇: {formatDateDDMMYYYY(startDate)}</p>
                                        </div>
                                    </div>
                                    <button 
                                        onClick={() => setShowDatePickerModal(false)} 
                                        className="p-1.5 rounded-full text-slate-400 hover:bg-slate-100 active-scale"
                                    >
                                        <Icon name="x" size={20} />
                                    </button>
                                </div>

                                {/* 快捷選擇按鈕 */}
                                <div className="flex gap-2">
                                    <button
                                        onClick={() => {
                                            const today = new Date().toISOString().split('T')[0];
                                            setStartDate(today);
                                            const d = new Date();
                                            setCalYear(d.getFullYear());
                                            setCalMonth(d.getMonth());
                                        }}
                                        className="flex-1 py-1.5 rounded-xl bg-indigo-50 text-indigo-700 text-xs font-bold hover:bg-indigo-100 transition-colors"
                                    >
                                        今天
                                    </button>
                                    <button
                                        onClick={() => {
                                            const tm = new Date();
                                            tm.setDate(tm.getDate() + 1);
                                            const tmIso = tm.toISOString().split('T')[0];
                                            setStartDate(tmIso);
                                            setCalYear(tm.getFullYear());
                                            setCalMonth(tm.getMonth());
                                        }}
                                        className="flex-1 py-1.5 rounded-xl bg-indigo-50 text-indigo-700 text-xs font-bold hover:bg-indigo-100 transition-colors"
                                    >
                                        明天
                                    </button>
                                    <button
                                        onClick={() => {
                                            const dat = new Date();
                                            dat.setDate(dat.getDate() + 2);
                                            const datIso = dat.toISOString().split('T')[0];
                                            setStartDate(datIso);
                                            setCalYear(dat.getFullYear());
                                            setCalMonth(dat.getMonth());
                                        }}
                                        className="flex-1 py-1.5 rounded-xl bg-indigo-50 text-indigo-700 text-xs font-bold hover:bg-indigo-100 transition-colors"
                                    >
                                        後天
                                    </button>
                                </div>

                                {/* 年月切換 Header */}
                                <div className="flex items-center justify-between px-2 py-1 bg-slate-50 rounded-2xl">
                                    <button 
                                        onClick={() => changeMonth(-1)} 
                                        className="p-2 rounded-xl text-slate-600 hover:bg-slate-200 active-scale"
                                    >
                                        <Icon name="chevron-left" size={18} />
                                    </button>
                                    <span className="text-sm font-black text-slate-800">
                                        {calYear} 年 {calMonth + 1} 月
                                    </span>
                                    <button 
                                        onClick={() => changeMonth(1)} 
                                        className="p-2 rounded-xl text-slate-600 hover:bg-slate-200 active-scale"
                                    >
                                        <Icon name="chevron-right" size={18} />
                                    </button>
                                </div>

                                {/* 日曆星期標頭 */}
                                <div className="grid grid-cols-7 text-center text-xs font-bold text-slate-400 pb-1">
                                    <span>日</span><span>一</span><span>二</span><span>三</span><span>四</span><span>五</span><span>六</span>
                                </div>

                                {/* 日曆天數 Grid */}
                                <div className="grid grid-cols-7 gap-1 text-center">
                                    {daysGrid.map((item, idx) => {
                                        const isSelected = item.dateStr === startDate;
                                        const isToday = item.dateStr === todayIso;

                                        let btnStyle = "text-slate-700 hover:bg-slate-100";
                                        if (!item.isCurrentMonth) btnStyle = "text-slate-300";
                                        if (isToday && !isSelected) btnStyle += " ring-2 ring-indigo-300 font-extrabold";
                                        if (isSelected) btnStyle = "bg-indigo-600 text-white font-black shadow-md shadow-indigo-200";

                                        return (
                                            <button
                                                key={idx}
                                                onClick={() => setStartDate(item.dateStr)}
                                                className={`h-9 w-full rounded-xl text-xs font-bold flex items-center justify-center transition-all active-scale ${btnStyle}`}
                                            >
                                                {item.day}
                                            </button>
                                        );
                                    })}
                                </div>

                                {/* 底部確定按鈕 */}
                                <div className="pt-2 border-t border-slate-100 flex items-center justify-center">
                                    <button
                                        onClick={() => setShowDatePickerModal(false)}
                                        className="w-full py-2.5 rounded-xl bg-indigo-600 text-white font-bold text-xs shadow-md shadow-indigo-100 hover:bg-indigo-700 active-scale"
                                    >
                                        確定
                                    </button>
                                </div>
                            </div>
                        </div>
                    )}

                    {/* ✨ 習慣達成率詳細統計報表彈窗 */}
                    {showStatsModal && (
                        <div className="fixed inset-0 z-50 overlay-blur flex items-center justify-center p-4 animate-pop">
                            <div className="bg-white rounded-3xl max-w-sm w-full p-6 shadow-2xl border border-slate-100 space-y-5 max-h-[90vh] overflow-y-auto no-scrollbar">
                                <div className="flex items-center justify-between border-b pb-3">
                                    <div className="flex items-center gap-2">
                                        <div className="p-2 bg-indigo-50 text-indigo-600 rounded-xl">
                                            <Icon name="bar-chart-2" size={20} />
                                        </div>
                                        <h3 className="text-lg font-black text-slate-800">習慣達成率詳細報表</h3>
                                    </div>
                                    <button onClick={() => setShowStatsModal(false)} className="p-1 rounded-full text-slate-400 hover:bg-slate-100">
                                        <Icon name="x" size={20} />
                                    </button>
                                </div>

                                {/* 頂部總結卡片 */}
                                <div className="bg-slate-50 p-4 rounded-2xl border border-slate-200/80 text-center space-y-2">
                                    <p className="text-xs font-bold text-slate-500">挑戰期間累積總達成率</p>
                                    <div className="text-4xl font-black text-indigo-600 tracking-tight">{stats.overallRate}%</div>
                                    <p className="text-xs text-slate-500 font-medium">
                                        已完成 <span className="font-bold text-slate-800">{stats.totalActualCompletions}</span> 次 / 應完成 {stats.totalPossibleCompletions} 次
                                    </p>
                                </div>

                                {/* 單項習慣達成率細節 */}
                                <div className="space-y-3">
                                    <h4 className="text-xs font-extrabold text-slate-400 tracking-wider uppercase">各項目打卡達成率</h4>
                                    <div className="space-y-3">
                                        {Array.from(selectedTasks).map(task => {
                                            const count = stats.perTaskStats[task] || 0;
                                            const rate = stats.elapsedDays > 0 ? Math.round((count / stats.elapsedDays) * 100) : 0;
                                            const activeTheme = DURATION_THEMES[planDuration] || DURATION_THEMES[7];

                                            return (
                                                <div key={task} className="space-y-1">
                                                    <div className="flex justify-between text-xs font-bold">
                                                        <span className="text-slate-700 truncate max-w-[200px]">{task}</span>
                                                        <span className={activeTheme.textAccent}>{count}/{stats.elapsedDays} 天 ({rate}%)</span>
                                                    </div>
                                                    <div className="w-full bg-slate-100 h-2 rounded-full overflow-hidden">
                                                        <div 
                                                            className={`${activeTheme.barFill} h-full rounded-full transition-all duration-500`}
                                                            style={{ width: `${rate}%` }}
                                                        ></div>
                                                    </div>
                                                </div>
                                            );
                                        })}
                                    </div>
                                </div>

                                <button
                                    onClick={() => setShowStatsModal(false)}
                                    className="w-full py-3 rounded-2xl bg-indigo-600 text-white font-bold active-scale"
                                >
                                    返回今日任務
                                </button>
                            </div>
                        </div>
                    )}

                    {/* 打卡儀式確認 Modal */}
                    {activeRitual && (
                        <div className="fixed inset-0 z-50 overlay-blur flex items-center justify-center p-4 animate-pop">
                            <div className="bg-white rounded-3xl max-w-sm w-full p-6 shadow-2xl border border-slate-100 space-y-4 text-center">
                                <div className="w-16 h-16 rounded-2xl bg-indigo-50 text-indigo-600 flex items-center justify-center mx-auto">
                                    <Icon name="sparkles" size={32} />
                                </div>
                                <div>
                                    <h3 className="text-lg font-black text-slate-800">{activeRitual.name}</h3>
                                    <p className="text-xs text-slate-500 mt-1">{activeRitual.hint}</p>
                                </div>
                                <div className="p-3 bg-slate-50 rounded-2xl text-xs font-semibold text-slate-600">
                                    準備好完成這項優質習慣了嗎？
                                </div>
                                <div className="flex gap-2">
                                    <button 
                                        onClick={() => setActiveRitual(null)}
                                        className="flex-1 py-3 rounded-2xl font-bold bg-slate-100 text-slate-600"
                                    >
                                        取消
                                    </button>
                                    <button 
                                        onClick={confirmRitual}
                                        className="flex-1 py-3 rounded-2xl font-black text-white bg-indigo-600 shadow-md active-scale"
                                    >
                                        確認完成
                                    </button>
                                </div>
                            </div>
                        </div>
                    )}

                    {/* 單項完成鼓勵 Toast */}
                    {showSingleEncouragement && (
                        <div className="fixed inset-0 z-50 overlay-blur flex items-center justify-center p-4 animate-pop">
                            <div className="bg-white rounded-3xl max-w-sm w-full p-6 shadow-2xl text-center space-y-4">
                                {mascotType === 'cloud' ? <SleepingCloudSVG className="mx-auto" /> : <GlowingStarSVG className="mx-auto" />}
                                <h3 className="text-xl font-black text-slate-800">你好叻! 請繼續下一項目標習慣。</h3>
                                <button 
                                    onClick={() => setShowSingleEncouragement(false)}
                                    className="w-full py-3 rounded-2xl bg-indigo-600 text-white font-bold active-scale"
                                >
                                    繼續保持
                                </button>
                            </div>
                        </div>
                    )}

                    {/* 全日任務達成大慶祝 Modal */}
                    {showSuccessToast && (
                        <div className="fixed inset-0 z-50 overlay-blur flex items-center justify-center p-4 animate-pop">
                            {confettiArray.map(c => (
                                <div 
                                    key={c.id} 
                                    className={`confetti-burst ${c.shape}`}
                                    style={{
                                        '--tx': c.tx, '--ty': c.ty, '--rot': c.rot,
                                        backgroundColor: c.color, width: c.size, height: c.size,
                                        left: '50%', top: '50%', animationDelay: c.delay
                                    }}
                                />
                            ))}
                            <div className="bg-white rounded-3xl max-w-sm w-full p-6 shadow-2xl text-center space-y-4 relative z-10">
                                <TrophySVG className="mx-auto" />
                                <h3 className="text-2xl font-black text-slate-800">所有目標習慣已經完成!</h3>
                                <button 
                                    onClick={() => setShowSuccessToast(false)}
                                    className="w-full py-3.5 rounded-2xl bg-emerald-500 text-white font-black shadow-lg shadow-emerald-200 active-scale"
                                >
                                    收下獎盃，明天再見!
                                </button>
                            </div>
                        </div>
                    )}

                    {/* 鬧鐘時間設定 Modal */}
                    {alarmSettingTask && (
                        <div className="fixed inset-0 z-50 overlay-blur flex items-center justify-center p-4 animate-pop">
                            <div className="bg-white rounded-3xl max-w-sm w-full p-6 shadow-2xl border border-slate-100 space-y-4">
                                <h3 className="text-base font-bold text-slate-800 flex items-center gap-2">
                                    <Icon name="bell" size={18} className="text-indigo-600" />
                                    設定「{alarmSettingTask}」提醒時間
                                </h3>
                                <input 
                                    type="time" 
                                    value={taskAlarms[alarmSettingTask] || "08:00"}
                                    onChange={(e) => setTaskAlarms({ ...taskAlarms, [alarmSettingTask]: e.target.value })}
                                    className="w-full p-3 rounded-2xl border-2 border-slate-200 text-center font-black text-xl text-slate-800 focus:border-indigo-600 focus:outline-none"
                                />
                                <div className="flex gap-2">
                                    <button 
                                        onClick={() => setAlarmSettingTask(null)}
                                        className="flex-1 py-3 rounded-2xl font-bold bg-slate-100 text-slate-600"
                                    >
                                        完成
                                    </button>
                                </div>
                            </div>
                        </div>
                    )}

                    {/* 重新設定計畫確認 Modal */}
                    {showResetConfirm && (
                        <div className="fixed inset-0 z-50 overlay-blur flex items-center justify-center p-4 animate-pop">
                            <div className="bg-white rounded-3xl max-w-sm w-full p-6 shadow-2xl border border-slate-100 space-y-4 text-center">
                                <div className="w-12 h-12 rounded-full bg-rose-100 text-rose-600 flex items-center justify-center mx-auto">
                                    <Icon name="alert-triangle" size={24} />
                                </div>
                                <h3 className="text-lg font-bold text-slate-800">重新開始睡眠挑戰？</h3>
                                <p className="text-xs text-slate-500">這將會清除目前的挑戰天數與打卡紀錄，並重置為最初設定狀態。</p>
                                <div className="flex gap-2">
                                    <button 
                                        onClick={() => setShowResetConfirm(false)}
                                        className="flex-1 py-3 rounded-2xl font-bold bg-slate-100 text-slate-600"
                                    >
                                        取消
                                    </button>
                                    <button 
                                        onClick={executeReset}
                                        className="flex-1 py-3 rounded-2xl font-bold text-white bg-rose-500 active-scale"
                                    >
                                        確認重置
                                    </button>
                                </div>
                            </div>
                        </div>
                    )}
                </div>
            );
        }

        const root = ReactDOM.createRoot(document.getElementById('root'));
        root.render(<App />);
    </script>
</body>
</html>

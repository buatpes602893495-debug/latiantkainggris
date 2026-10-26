<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TKA Bahasa Inggris 2025 - Quizizz Arcade</title>
    <!-- JS Confetti Library -->
    <script src="https://cdn.jsdelivr.net/npm/js-confetti@latest/dist/js-confetti.browser.js"></script>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;500;600;700&family=Plus+Jakarta+Sans:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    
    <style>
        /* Standalone CSS Styles & Layout */
        *, ::before, ::after { box-sizing: border-box; margin: 0; padding: 0; }
        
        body { 
            font-family: 'Plus Jakarta Sans', sans-serif; 
            background-color: #020617; 
            color: #ffffff; 
            min-height: 100vh; 
            display: flex; 
            align-items: center; 
            justify-content: center; 
            padding: 0.75rem; 
            user-select: none; 
            overflow-x: hidden; 
        }

        .font-heading { font-family: 'Fredoka', cursive, sans-serif; }

        /* Helper Utilities */
        .hidden { display: none !important; }
        .flex { display: flex !important; }
        .grid { display: grid !important; }

        /* Card Container */
        #app {
            width: 100%;
            max-width: 56rem;
            background-color: #0f172a;
            border: 4px solid #1e293b;
            border-radius: 1.5rem;
            box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.5);
            overflow: hidden;
            position: relative;
            min-height: 640px;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        /* 3D Quizizz Button Styles */
        .btn-quizizz-purple {
            background-color: #8b5cf6;
            box-shadow: 0 6px 0 0 #6d28d9;
            transition: all 0.1s ease;
            color: #ffffff;
            font-weight: 900;
            border-radius: 1rem;
            cursor: pointer;
            border: none;
        }
        .btn-quizizz-purple:active:not(:disabled) {
            transform: translateY(4px);
            box-shadow: 0 2px 0 0 #6d28d9;
        }

        .btn-quizizz-green {
            background-color: #10b981;
            box-shadow: 0 6px 0 0 #047857;
            transition: all 0.1s ease;
            color: #ffffff;
            font-weight: 900;
            border-radius: 1rem;
            cursor: pointer;
            border: none;
        }
        .btn-quizizz-green:active:not(:disabled) {
            transform: translateY(4px);
            box-shadow: 0 2px 0 0 #047857;
        }

        .option-card {
            box-shadow: 0 6px 0 0 rgba(0, 0, 0, 0.25);
            transition: transform 0.12s ease, box-shadow 0.12s ease, background-color 0.2s;
            padding: 1rem;
            border-radius: 1rem;
            font-weight: 700;
            text-align: left;
            display: flex;
            align-items: center;
            justify-content: space-between;
            border-bottom: 4px solid rgba(0,0,0,0.3);
            cursor: pointer;
        }
        .option-card:hover:not(:disabled) {
            transform: translateY(-3px);
            box-shadow: 0 9px 0 0 rgba(0, 0, 0, 0.25);
        }
        .option-card:active:not(:disabled) {
            transform: translateY(3px);
            box-shadow: 0 3px 0 0 rgba(0, 0, 0, 0.25);
        }

        /* Option Colors */
        .opt-rose { background-color: #e11d48; color: #fff; }
        .opt-rose:hover { background-color: #f43f5e; }
        .opt-sky { background-color: #0284c7; color: #fff; }
        .opt-sky:hover { background-color: #38bdf8; }
        .opt-amber { background-color: #d97706; color: #fff; }
        .opt-amber:hover { background-color: #fbbf24; }
        .opt-emerald { background-color: #059669; color: #fff; }
        .opt-emerald:hover { background-color: #34d399; }

        /* Animations */
        @keyframes pulse-shake {
            0%, 100% { transform: scale(1) rotate(0deg); }
            20% { transform: scale(1.15) rotate(-6deg); }
            40% { transform: scale(1.15) rotate(6deg); }
            60% { transform: scale(1.1) rotate(-3deg); }
        }
        .animate-shake { animation: pulse-shake 0.4s ease-in-out; }

        @keyframes float-slow {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }
        .animate-float { animation: float-slow 3s ease-in-out infinite; }

        /* Typography & Layout Helpers */
        .text-gradient {
            background: linear-gradient(to right, #c084fc, #f472b6, #fcd34d);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .grid-options {
            display: grid;
            grid-template-columns: 1fr;
            gap: 0.75rem;
        }
        @media (min-width: 640px) {
            .grid-options { grid-template-columns: 1fr 1fr; }
        }

        ::-webkit-scrollbar { width: 8px; }
        ::-webkit-scrollbar-track { background: #1e1b4b; }
        ::-webkit-scrollbar-thumb { background: #4c1d95; border-radius: 4px; }
    </style>
</head>
<body>

    <canvas id="confetti-canvas" style="position:fixed; inset:0; pointer-events:none; z-index:50;"></canvas>

    <div id="app">
        <!-- AUDIO TOGGLE BUTTON -->
        <div style="position: absolute; top: 1rem; right: 1rem; z-index: 20;">
            <button onclick="toggleSound()" id="sound-toggle-btn" style="background: rgba(30,41,59,0.8); border: 2px solid #334155; color: #fbbf24; padding: 0.5rem 0.75rem; border-radius: 1rem; cursor: pointer;">
                <span id="sound-icon" style="font-size: 1.25rem;">🔊</span>
            </button>
        </div>

        <!-- WELCOME SCREEN -->
        <div id="welcome-screen" style="padding: 2rem; text-align: center; margin: auto; display: flex; flex-direction: column; align-items: center;">
            <div class="animate-float" style="margin-bottom: 1rem; font-size: 4rem;">🎮</div>
            <div style="background: rgba(168,85,247,0.2); border: 1px solid rgba(168,85,247,0.4); color: #d8b4fe; padding: 0.35rem 1rem; border-radius: 9999px; font-size: 0.875rem; font-weight: 700; margin-bottom: 1rem;">
                🔥 SIMULASI TKA BAHASA INGGRIS 2025
            </div>
            <h1 class="font-heading text-gradient" style="font-size: 3rem; font-weight: 900; margin-bottom: 0.75rem;">
                ENGLISH ARENA
            </h1>
            <p style="color: #cbd5e1; margin-bottom: 2rem; max-width: 28rem; font-size: 0.95rem; line-height: 1.5;">
                Uji kemampuan membaca, tata bahasa, dan kosakatamu dalam 30 soal interaktif berhadiah Combo Streak dan Poin!
            </p>

            <div style="background: rgba(30,41,59,0.9); border: 2px solid #334155; padding: 1rem; border-radius: 1rem; margin-bottom: 2rem; width: 100%; max-width: 28rem; text-align: left;">
                <span style="font-size: 0.75rem; font-weight: 800; text-transform: uppercase; color: #94a3b8; display: block; margin-bottom: 0.5rem;">Pilih Mode Permainan:</span>
                <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 0.75rem;">
                    <button onclick="setMode('instant')" id="mode-instant-btn" style="padding: 0.75rem; border-radius: 0.75rem; border: 2px solid #a855f7; background: rgba(168,85,247,0.2); color: #e9d5ff; font-weight: 700; font-size: 0.85rem; cursor: pointer;">
                        ⚡ Instant Feedback<br><span style="font-size: 0.65rem; font-weight: 400; color: #cbd5e1;">(Langsung tahu benar/salah)</span>
                    </button>
                    <button onclick="setMode('exam')" id="mode-exam-btn" style="padding: 0.75rem; border-radius: 0.75rem; border: 2px solid #334155; background: #0f172a; color: #94a3b8; font-weight: 700; font-size: 0.85rem; cursor: pointer;">
                        📝 Test Mode<br><span style="font-size: 0.65rem; font-weight: 400; color: #64748b;">(Pembahasan di akhir)</span>
                    </button>
                </div>
            </div>

            <button onclick="startQuiz()" class="btn-quizizz-purple font-heading" style="width: 100%; max-width: 28rem; font-size: 1.5rem; padding: 1rem; border-bottom: 4px solid #4c1d95;">
                MULAI GAME! 🚀
            </button>
        </div>

        <!-- QUIZ SCREEN -->
        <div id="quiz-screen" class="hidden" style="flex-direction: column; justify-content: space-between; height: 100%; padding: 1.5rem;">
            <div>
                <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 0.75rem;">
                    <div id="question-badge" class="font-heading" style="background: rgba(88,28,135,0.8); border: 2px solid rgba(168,85,247,0.4); color: #d8b4fe; padding: 0.35rem 1rem; border-radius: 1rem; font-size: 0.85rem; font-weight: 700;">
                        🎯 <span id="q-counter-text">SOAL 1 / 30</span>
                    </div>

                    <div style="display: flex; align-items: center; gap: 0.5rem;">
                        <div id="streak-box" class="hidden" style="background: rgba(245,158,11,0.2); border: 2px solid rgba(245,158,11,0.5); color: #fcd34d; padding: 0.25rem 0.75rem; border-radius: 1rem; font-size: 0.85rem; font-weight: 900; align-items: center; gap: 0.25rem;">
                            🔥 <span id="streak-count">0</span> STREAK!
                        </div>
                        <div style="background: rgba(49,46,129,0.8); border: 2px solid rgba(99,102,241,0.4); color: #a5b4fc; padding: 0.25rem 0.85rem; border-radius: 1rem; font-size: 0.85rem; font-weight: 900;">
                            💎 <span id="score-display">0</span> PTS
                        </div>
                        <div style="background: #1e293b; border: 2px solid #334155; color: #fbbf24; padding: 0.25rem 0.85rem; border-radius: 1rem; font-size: 0.85rem; font-family: monospace; font-weight: 700;">
                            ⏱️ <span id="timer-display">00:00</span>
                        </div>
                    </div>
                </div>

                <div style="width: 100%; background: #020617; height: 0.85rem; border-radius: 9999px; margin-bottom: 1.25rem; overflow: hidden; border: 2px solid #1e293b; padding: 2px;">
                    <div id="progress-bar" style="background: linear-gradient(to right, #a855f7, #ec4899, #fbbf24); height: 100%; border-radius: 9999px; width: 3.33%; transition: width 0.3s ease;"></div>
                </div>
            </div>

            <div style="margin: auto 0; display: flex; flex-direction: column; gap: 1rem;">
                <div id="passage-container" class="hidden" style="background: rgba(2,6,23,0.7); border-left: 4px solid #a855f7; padding: 1rem; border-radius: 1rem; color: #cbd5e1; font-size: 0.85rem; line-height: 1.5; max-height: 11rem; overflow-y: auto; border-top: 1px solid #1e293b; border-right: 1px solid #1e293b; border-bottom: 1px solid #1e293b;">
                    <p id="passage-text" style="font-style: italic; whitespace: pre-line;"></p>
                </div>

                <h2 id="question-text" style="font-size: 1.15rem; font-weight: 700; color: #fff; line-height: 1.4;">
                    Loading Question...
                </h2>

                <div id="options-container" class="grid-options"></div>

                <div id="feedback-banner" class="hidden" style="padding: 1rem; border-radius: 1rem; border: 2px solid transparent; font-size: 0.875rem; font-weight: 700; display: flex; align-items: flex-start; gap: 0.75rem;">
                    <span id="feedback-icon" style="font-size: 1.5rem;"></span>
                    <div>
                        <div id="feedback-title" class="font-heading" style="font-size: 1.1rem;"></div>
                        <div id="feedback-text" style="font-weight: 400; font-size: 0.85rem; color: #e2e8f0; margin-top: 0.25rem;"></div>
                    </div>
                </div>
            </div>

            <div style="display: flex; justify-between: space-between; align-items: center; padding-top: 1rem; margin-top: 0.5rem; border-top: 1px solid #1e293b;">
                <button id="prev-btn" onclick="prevQuestion()" style="padding: 0.6rem 1.25rem; border-radius: 0.75rem; border: 2px solid #1e293b; background: transparent; color: #94a3b8; font-weight: 700; cursor: pointer;">
                    ← Sebelumnya
                </button>
                
                <button id="next-btn" onclick="nextQuestion()" class="btn-quizizz-purple font-heading" style="padding: 0.6rem 1.5rem; font-size: 0.9rem;">
                    Selanjutnya →
                </button>
            </div>
        </div>

        <!-- RESULT SCREEN -->
        <div id="result-screen" class="hidden" style="padding: 2rem; text-align: center; margin: auto; display: flex; flex-direction: column; align-items: center;">
            <div id="result-emoji" class="animate-bounce" style="font-size: 4rem; margin-bottom: 0.5rem;">🏆</div>
            <h2 id="result-title" class="font-heading" style="font-size: 2.5rem; font-weight: 900; color: #fff; margin-bottom: 0.5rem;">LUAR BIASA!</h2>
            <p id="result-subtitle" style="color: #94a3b8; margin-bottom: 1.5rem; font-size: 0.95rem;">Kamu telah menyelesaikan simulasi TKA Bahasa Inggris 2025.</p>

            <div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 0.75rem; width: 100%; max-width: 32rem; margin-bottom: 2rem;">
                <div style="background: rgba(30,41,59,0.9); border: 2px solid rgba(168,85,247,0.4); padding: 1rem; border-radius: 1rem; text-align: center;">
                    <span style="font-size: 0.65rem; color: #94a3b8; font-weight: 800; text-transform: uppercase; display: block; margin-bottom: 0.25rem;">Total Skor</span>
                    <span id="final-score" class="font-heading" style="font-size: 2.25rem; font-weight: 900; color: #c084fc;">0</span>
                </div>
                <div style="background: rgba(30,41,59,0.9); border: 2px solid rgba(16,185,129,0.4); padding: 1rem; border-radius: 1rem; text-align: center;">
                    <span style="font-size: 0.65rem; color: #94a3b8; font-weight: 800; text-transform: uppercase; display: block; margin-bottom: 0.25rem;">Akurasi</span>
                    <span id="final-accuracy" class="font-heading" style="font-size: 2.25rem; font-weight: 900; color: #34d399;">0%</span>
                </div>
                <div style="background: rgba(30,41,59,0.9); border: 2px solid rgba(245,158,11,0.4); padding: 1rem; border-radius: 1rem; text-align: center;">
                    <span style="font-size: 0.65rem; color: #94a3b8; font-weight: 800; text-transform: uppercase; display: block; margin-bottom: 0.25rem;">Max Streak</span>
                    <span id="max-streak-display" class="font-heading" style="font-size: 2.25rem; font-weight: 900; color: #fbbf24;">0 🔥</span>
                </div>
            </div>

            <div style="display: flex; gap: 0.75rem; width: 100%; max-width: 28rem;">
                <button onclick="showReview()" class="btn-quizizz-purple font-heading" style="width: 100%; padding: 0.85rem; font-size: 1rem;">
                    🔍 LIHAT PEMBAHASAN
                </button>
                <button onclick="restartQuiz()" style="width: 100%; background: #1e293b; color: #e2e8f0; border: 2px solid #334155; font-family: 'Fredoka', sans-serif; font-weight: 700; border-radius: 1rem; cursor: pointer; padding: 0.85rem; font-size: 1rem;">
                    🔄 MAIN LAGI
                </button>
            </div>
        </div>

        <!-- REVIEW SCREEN -->
        <div id="review-screen" class="hidden" style="padding: 1.5rem; height: 100%; flex-direction: column;">
            <div style="display: flex; justify-content: space-between; align-items: center; padding-bottom: 1rem; margin-bottom: 1rem; border-bottom: 1px solid #1e293b;">
                <div>
                    <h2 class="font-heading" style="font-size: 1.5rem; font-weight: 700; color: #fff;">Pembahasan Soal Lengkap</h2>
                    <p style="font-size: 0.75rem; color: #94a3b8;">Evaluasi menyeluruh untuk tiap butir soal TKA.</p>
                </div>
                <button onclick="backToResult()" style="font-size: 0.85rem; background: #1e293b; color: #cbd5e1; font-weight: 700; padding: 0.5rem 1rem; border-radius: 0.75rem; border: 1px solid #334155; cursor: pointer;">
                    Kembali ke Skor
                </button>
            </div>

            <div id="review-list" style="display: flex; flex-direction: column; gap: 1rem; overflow-y: auto; max-height: 26rem; padding-right: 0.5rem;"></div>
        </div>
    </div>

    <script>
        // WEB AUDIO SYNTHESIZER
        let soundEnabled = true;
        const audioCtx = new (window.AudioContext || window.webkitAudioContext)();

        function playSound(type) {
            if (!soundEnabled) return;
            if (audioCtx.state === 'suspended') audioCtx.resume();

            const osc = audioCtx.createOscillator();
            const gain = audioCtx.createGain();
            osc.connect(gain);
            gain.connect(audioCtx.destination);

            const now = audioCtx.currentTime;

            if (type === 'pop') {
                osc.type = 'sine';
                osc.frequency.setValueAtTime(400, now);
                osc.frequency.exponentialRampToValueAtTime(800, now + 0.08);
                gain.gain.setValueAtTime(0.2, now);
                gain.gain.exponentialRampToValueAtTime(0.01, now + 0.08);
                osc.start(now);
                osc.stop(now + 0.08);
            } else if (type === 'correct') {
                osc.type = 'triangle';
                osc.frequency.setValueAtTime(523.25, now);
                osc.frequency.setValueAtTime(659.25, now + 0.08);
                osc.frequency.setValueAtTime(783.99, now + 0.16);
                gain.gain.setValueAtTime(0.25, now);
                gain.gain.exponentialRampToValueAtTime(0.01, now + 0.3);
                osc.start(now);
                osc.stop(now + 0.3);
            } else if (type === 'wrong') {
                osc.type = 'sawtooth';
                osc.frequency.setValueAtTime(220, now);
                osc.frequency.setValueAtTime(180, now + 0.12);
                gain.gain.setValueAtTime(0.3, now);
                gain.gain.exponentialRampToValueAtTime(0.01, now + 0.3);
                osc.start(now);
                osc.stop(now + 0.3);
            } else if (type === 'finish') {
                osc.type = 'sine';
                osc.frequency.setValueAtTime(523.25, now);
                osc.frequency.setValueAtTime(659.25, now + 0.1);
                osc.frequency.setValueAtTime(783.99, now + 0.2);
                osc.frequency.setValueAtTime(1046.50, now + 0.3);
                gain.gain.setValueAtTime(0.3, now);
                gain.gain.exponentialRampToValueAtTime(0.01, now + 0.5);
                osc.start(now);
                osc.stop(now + 0.5);
            }
        }

        function toggleSound() {
            soundEnabled = !soundEnabled;
            document.getElementById('sound-icon').innerText = soundEnabled ? '🔊' : '🔇';
        }

        const jsConfetti = new JSConfetti();
        function triggerConfetti() {
            jsConfetti.addConfetti({
                emojis: ['🎉', '⭐', '🔥', '✨', '🎓'],
                emojiSize: 40,
                confettiNumber: 60,
            });
        }

        // 30 SOAL TKA BAHASA INGGRIS
        const questions = [
            {
                passage: "Read the text to answer questions 1 to 5:\n\n'A new study reveals that high school students who sleep fewer than seven hours per night exhibit significantly lower academic performance. Sleep deprivation negatively impacts memory consolidation, critical thinking, and emotional resilience. Sleep experts strongly advise maintaining a consistent bedtime routine and eliminating screen exposure at least 60 minutes prior to sleep.'",
                question: "1. What is the primary focus of the passage?",
                options: [
                    "The benefits of night-time studying for exams.",
                    "The harmful effects of inadequate sleep on student performance.",
                    "How screen time enhances memory retention in teenagers.",
                    "Methods for diagnosing severe insomnia in high schools."
                ],
                correct: 1,
                explanation: "Teks berfokus membahas bagaimana kurang tidur (sleep deprivation) berdampak negatif terhadap performa akademis siswa."
            },
            {
                passage: "Refer to Text 1.",
                question: "2. According to the text, how much sleep is recommended to maintain optimal performance?",
                options: [
                    "Under 5 hours daily",
                    "Exactly 6 hours daily",
                    "Seven hours or more daily",
                    "Around 4 to 6 hours daily"
                ],
                correct: 2,
                explanation: "Teks menyebutkan bahwa siswa yang tidur 'fewer than seven hours' memiliki performa lebih rendah, sehingga disarankan tidur 7 jam atau lebih."
            },
            {
                passage: "Refer to Text 1.",
                question: "3. The word 'deprivation' in the text is closest in meaning to...",
                options: [
                    "Abundance",
                    "Lack",
                    "Quality",
                    "Extension"
                ],
                correct: 1,
                explanation: "'Deprivation' berarti kekurangan/kehilangan, yang bersinonim dengan kata 'lack'."
            },
            {
                passage: "Refer to Text 1.",
                question: "4. Which of the following is NOT listed as a consequence of sleep loss?",
                options: [
                    "Impaired memory consolidation",
                    "Reduced critical thinking skills",
                    "Weaker emotional resilience",
                    "Increased physical height"
                ],
                correct: 3,
                explanation: "Pertumbuhan tinggi badan ('increased physical height') tidak disebutkan dalam teks sebagai dampak kurang tidur."
            },
            {
                passage: "Refer to Text 1.",
                question: "5. What do experts suggest regarding electronic devices before sleeping?",
                options: [
                    "Keep screens on for relaxing music",
                    "Avoid screens for at least one hour before bed",
                    "Use screens only for reading digital books",
                    "Charge screens next to the bed"
                ],
                correct: 1,
                explanation: "Teks menyatakan 'eliminating screen exposure at least 60 minutes prior to sleep'."
            },
            {
                passage: "Read the text to answer questions 6 to 10:\n\n'Renewable energy sources such as solar, wind, and hydroelectric power are becoming vital components in combatting global climate change. Unlike fossil fuels, which discharge harmful greenhouse gases and exhaust finite natural reserves, clean energy systems offer sustainable alternatives that protect ecological balance for future generations.'",
                question: "6. What advantage of renewable energy over fossil fuels is emphasized?",
                options: [
                    "It consumes natural reserves faster.",
                    "It releases controlled amounts of greenhouse gases.",
                    "It is sustainable and does not pollute with harmful emissions.",
                    "It requires no financial investment."
                ],
                correct: 2,
                explanation: "Teks menekankan bahwa energi terbarukan menyediakan alternatif yang berkelanjutan tanpa membuang gas rumah kaca yang berbahaya."
            },
            {
                passage: "Refer to Text 2.",
                question: "7. The word 'exhaust' in the passage means...",
                options: [
                    "Deplete or run out of",
                    "Energize or restore",
                    "Clean or purify",
                    "Expand or enlarge"
                ],
                correct: 0,
                explanation: "Dalam konteks sumber daya alam terbatas ('finite reserves'), kata 'exhaust' berarti menguras atau menghabiskan (deplete)."
            },
            {
                passage: "Refer to Text 2.",
                question: "8. Which energy sources are mentioned as clean energy?",
                options: [
                    "Coal, gas, and oil",
                    "Solar, wind, and hydro power",
                    "Nuclear and diesel",
                    "Kerosene and natural gas"
                ],
                correct: 1,
                explanation: "Teks secara eksplisit menyebutkan 'solar, wind, and hydroelectric power'."
            },
            {
                passage: "Refer to Text 2.",
                question: "9. Why are fossil fuels considered harmful?",
                options: [
                    "Because they are unlimited",
                    "Because they emit greenhouse gases and deplete finite resources",
                    "Because they promote ecological balance",
                    "Because they produce zero carbon emissions"
                ],
                correct: 1,
                explanation: "Teks menyebutkan 'fossil fuels, which discharge harmful greenhouse gases and exhaust finite natural reserves'."
            },
            {
                passage: "Refer to Text 2.",
                question: "10. What is the author's overall tone regarding clean energy?",
                options: [
                    "Skeptical",
                    "Neutral",
                    "Supportive and favorable",
                    "Dismissive"
                ],
                correct: 2,
                explanation: "Penulis menilai energi terbarukan sebagai elemen vital dan positif bagi masa depan (supportive/favorable)."
            },
            {
                passage: "Read the text to answer questions 11 to 15:\n\n'Digital literacy is no longer an optional luxury; it is a fundamental requirement in modern career pathways. Employees capable of navigating complex software, analyzing big data, and protecting online communications enjoy far higher employability rates than those who rely solely on conventional skills.'",
                question: "11. What is the primary message of the text?",
                options: [
                    "Traditional skills are completely useless today.",
                    "Digital literacy is essential for modern career success.",
                    "Programming skills are only required for computer scientists.",
                    "Modern companies avoid using digital platforms."
                ],
                correct: 1,
                explanation: "Pesan utama teks adalah literasi digital kini merupakan kebutuhan mendasar (fundamental requirement) dalam karir modern."
            },
            {
                passage: "Refer to Text 3.",
                question: "12. The word 'fundamental' is closest in meaning to...",
                options: [
                    "Unimportant",
                    "Essential",
                    "Secondary",
                    "Temporary"
                ],
                correct: 1,
                explanation: "'Fundamental' berarti mendasar atau sangat penting (essential)."
            },
            {
                passage: "Refer to Text 3.",
                question: "13. What benefit do digitally literate workers receive?",
                options: [
                    "Higher employability rates",
                    "Lower workload expectations",
                    "Exemption from teamwork",
                    "Guaranteed executive status"
                ],
                correct: 0,
                explanation: "Teks menyebutkan mereka 'enjoy far higher employability rates'."
            },
            {
                passage: "Refer to Text 3.",
                question: "14. Which skill is NOT listed as part of digital literacy in the text?",
                options: [
                    "Navigating complex software",
                    "Analyzing big data",
                    "Protecting online communications",
                    "Designing physical machinery"
                ],
                correct: 3,
                explanation: "Perancangan mesin fisik ('designing physical machinery') tidak disebutkan dalam daftar literasi digital pada teks."
            },
            {
                passage: "Refer to Text 3.",
                question: "15. What is the antonym of 'conventional' as used in the passage?",
                options: [
                    "Traditional",
                    "Modern / Innovative",
                    "Standard",
                    "Usual"
                ],
                correct: 1,
                explanation: "'Conventional' berarti konvensional/tradisional. Lawan katanya adalah modern atau inovatif."
            },
            {
                passage: null,
                question: "16. Grammar: If I ___ earlier, I would not have missed the main presentation.",
                options: [
                    "arrive",
                    "arrived",
                    "had arrived",
                    "have arrived"
                ],
                correct: 2,
                explanation: "Conditional Sentence Type 3 (pengandaian masa lalu): If + Subject + had + V3, Subject + would have + V3."
            },
            {
                passage: null,
                question: "17. Grammar: The groundbreaking project ___ by the research team before the deadline next week.",
                options: [
                    "will complete",
                    "will be completed",
                    "has completed",
                    "was completed"
                ],
                correct: 1,
                explanation: "Bentuk pasif masa depan (Future Passive): 'will be completed' karena subjek berupa benda (project) yang dikerjakan."
            },
            {
                passage: null,
                question: "18. Grammar: She is the researcher ___ study on artificial intelligence was published in Nature magazine.",
                options: [
                    "who",
                    "whom",
                    "whose",
                    "which"
                ],
                correct: 2,
                explanation: "Menggunakan relative pronoun 'whose' untuk menyatakan kepemilikan (penelitian milik peneliti tersebut)."
            },
            {
                passage: null,
                question: "19. Grammar: Despite ___ very tired after the long journey, he stayed up to finish his report.",
                options: [
                    "feel",
                    "feeling",
                    "felt",
                    "he feels"
                ],
                correct: 1,
                explanation: "Preposisi 'Despite' harus diikuti oleh Gerund (V-ing) yaitu 'feeling'."
            },
            {
                passage: null,
                question: "20. Grammar: Neither the manager nor the staff members ___ aware of the upcoming policy revision.",
                options: [
                    "was",
                    "were",
                    "is",
                    "has been"
                ],
                correct: 1,
                explanation: "Dalam struktur 'neither... nor...', kata kerja (verb) mengikuti subjek terdekat (staff members = jamak) -> 'were'."
            },
            {
                passage: "Read the text to answer questions 21 to 25:\n\n'Urban farming is gaining widespread momentum in densely populated cities worldwide. By transforming vacant rooftops, balconies, and unused community plots into green gardens, urban citizens can cultivate fresh organic vegetables locally. This practice not only reduces carbon footprints caused by long-distance food transport but also fosters community bonding.'",
                question: "21. What is the main idea of the text?",
                options: [
                    "Why rural farming is declining rapidly.",
                    "The growth and benefits of urban farming in cities.",
                    "How food transportation creates profitable businesses.",
                    "The process of buying vacant real estate."
                ],
                correct: 1,
                explanation: "Teks menjelaskan pertumbuhan dan berbagai manfaat dari pertanian perkotaan (urban farming)."
            },
            {
                passage: "Refer to Text 4.",
                question: "22. How does urban farming help reduce carbon footprints?",
                options: [
                    "By replacing vehicles with bikes",
                    "By shortening food transport distances",
                    "By using artificial lighting indoors",
                    "By exporting food overseas"
                ],
                correct: 1,
                explanation: "Teks menyatakan 'reduces carbon footprints caused by long-distance food transport' karena makanan ditanam lokal."
            },
            {
                passage: "Refer to Text 4.",
                question: "23. The word 'vacant' in the passage means...",
                options: [
                    "Occupied",
                    "Empty / Unused",
                    "Expensive",
                    "Crowded"
                ],
                correct: 1,
                explanation: "'Vacant' berarti kosong atau tidak terpakai (empty/unused)."
            },
            {
                passage: "Refer to Text 4.",
                question: "24. Where do urban residents establish these gardens?",
                options: [
                    "On rooftops, balconies, and community plots",
                    "In deep underground tunnels",
                    "On highway lanes",
                    "Inside shopping malls"
                ],
                correct: 0,
                explanation: "Teks menyebutkan 'vacant rooftops, balconies, and unused community plots'."
            },
            {
                passage: "Refer to Text 4.",
                question: "25. Which social benefit of urban farming is highlighted?",
                options: [
                    "Decreasing city noise levels",
                    "Fostering community bonding",
                    "Eliminating urban tax rates",
                    "Increasing apartment prices"
                ],
                correct: 1,
                explanation: "Teks secara spesifik menyatakan 'fosters community bonding'."
            },
            {
                passage: null,
                question: "26. Vocabulary: The company decided to ___ its investments into green technology starting next quarter.",
                options: [
                    "diversify",
                    "divert",
                    "divide",
                    "diminish"
                ],
                correct: 0,
                explanation: "'Diversify' berarti memvariasikan/mengembangkan investasi ke sektor baru (green technology)."
            },
            {
                passage: null,
                question: "27. Collocation: 'The board members finally arrived ___ a consensus after hours of deliberation.'",
                options: [
                    "to",
                    "at",
                    "in",
                    "on"
                ],
                correct: 1,
                explanation: "Pasangan frasa kata kerja yang tepat adalah 'arrive at a consensus' (mencapai kesepakatan)."
            },
            {
                passage: null,
                question: "28. Vocabulary: Her presentation was so ___ that even complex technical details became easy to understand.",
                options: [
                    "ambiguous",
                    "lucid",
                    "obscure",
                    "redundant"
                ],
                correct: 1,
                explanation: "'Lucid' berarti sangat jelas dan mudah dipahami."
            },
            {
                passage: null,
                question: "29. Synonym: What is the synonym for 'mitigate'?",
                options: [
                    "Intensify",
                    "Alleviate / Reduce",
                    "Aggravate",
                    "Neglect"
                ],
                correct: 1,
                explanation: "'Mitigate' berarti meringankan atau mengurangi dampak negatif, bersinonim dengan 'alleviate'."
            },
            {
                passage: null,
                question: "30. Inversion: 'Hardly had the meeting started ___ the power went out.'",
                options: [
                    "than",
                    "when",
                    "then",
                    "after"
                ],
                correct: 1,
                explanation: "Pola inversi 'Hardly had + Subjek + V3' secara berpasangan selalu diikuti oleh 'when'."
            }
        ];

        let currentIdx = 0;
        let gameMode = 'instant';
        let userAnswers = new Array(questions.length).fill(null);
        let score = 0;
        let currentStreak = 0;
        let maxStreak = 0;
        let timerInterval;
        let secondsElapsed = 0;

        function setMode(mode) {
            gameMode = mode;
            playSound('pop');
            const instantBtn = document.getElementById('mode-instant-btn');
            const examBtn = document.getElementById('mode-exam-btn');

            if (mode === 'instant') {
                instantBtn.style.border = "2px solid #a855f7";
                instantBtn.style.background = "rgba(168,85,247,0.2)";
                instantBtn.style.color = "#e9d5ff";

                examBtn.style.border = "2px solid #334155";
                examBtn.style.background = "#0f172a";
                examBtn.style.color = "#94a3b8";
            } else {
                examBtn.style.border = "2px solid #a855f7";
                examBtn.style.background = "rgba(168,85,247,0.2)";
                examBtn.style.color = "#e9d5ff";

                instantBtn.style.border = "2px solid #334155";
                instantBtn.style.background = "#0f172a";
                instantBtn.style.color = "#94a3b8";
            }
        }

        function startQuiz() {
            playSound('pop');
            document.getElementById('welcome-screen').classList.add('hidden');
            document.getElementById('quiz-screen').classList.remove('hidden');
            document.getElementById('quiz-screen').classList.add('flex');
            startTimer();
            renderQuestion();
        }

        function startTimer() {
            timerInterval = setInterval(() => {
                secondsElapsed++;
                const mins = Math.floor(secondsElapsed / 60).toString().padStart(2, '0');
                const secs = (secondsElapsed % 60).toString().padStart(2, '0');
                document.getElementById('timer-display').innerText = `${mins}:${secs}`;
            }, 1000);
        }

        function renderQuestion() {
            const q = questions[currentIdx];

            document.getElementById('q-counter-text').innerText = `SOAL ${currentIdx + 1} / ${questions.length}`;
            document.getElementById('progress-bar').style.width = `${((currentIdx + 1) / questions.length) * 100}%`;
            document.getElementById('score-display').innerText = Math.round(score);

            const streakBox = document.getElementById('streak-box');
            if (currentStreak >= 2) {
                streakBox.classList.remove('hidden');
                streakBox.classList.add('flex');
                document.getElementById('streak-count').innerText = currentStreak;
            } else {
                streakBox.classList.add('hidden');
                streakBox.classList.remove('flex');
            }

            const passageContainer = document.getElementById('passage-container');
            if (q.passage) {
                document.getElementById('passage-text').innerText = q.passage;
                passageContainer.classList.remove('hidden');
            } else {
                passageContainer.classList.add('hidden');
            }

            document.getElementById('question-text').innerText = q.question;
            document.getElementById('feedback-banner').classList.add('hidden');

            const optionsContainer = document.getElementById('options-container');
            optionsContainer.innerHTML = '';

            const optionClasses = ['opt-rose', 'opt-sky', 'opt-amber', 'opt-emerald'];
            const answered = userAnswers[currentIdx] !== null;

            q.options.forEach((opt, idx) => {
                const btn = document.createElement('button');
                btn.disabled = answered && gameMode === 'instant';

                let cardClass = optionClasses[idx % 4];
                let iconMarker = '';

                if (answered) {
                    if (gameMode === 'instant') {
                        if (idx === q.correct) {
                            cardClass = "";
                            btn.style.background = "#10b981";
                            btn.style.color = "#fff";
                            btn.style.outline = "4px solid #6ee7b7";
                            iconMarker = '✔';
                        } else if (idx === userAnswers[currentIdx]) {
                            cardClass = "";
                            btn.style.background = "#e11d48";
                            btn.style.color = "#fff";
                            btn.style.outline = "4px solid #fca5a5";
                            iconMarker = '✖';
                        } else {
                            cardClass = "";
                            btn.style.background = "#1e293b";
                            btn.style.color = "#64748b";
                            btn.style.opacity = "0.4";
                        }
                    } else {
                        if (idx === userAnswers[currentIdx]) {
                            cardClass = "";
                            btn.style.background = "#9333ea";
                            btn.style.color = "#fff";
                            btn.style.outline = "4px solid #d8b4fe";
                            iconMarker = '📌';
                        } else {
                            cardClass = "";
                            btn.style.background = "#1e293b";
                            btn.style.color = "#cbd5e1";
                        }
                    }
                }

                btn.className = `option-card ${cardClass}`;
                btn.onclick = () => handleOptionClick(idx);

                btn.innerHTML = `
                    <span style="display:flex; align-items:center; gap:0.75rem;">
                        <span class="font-heading" style="background:rgba(0,0,0,0.2); padding:0.25rem 0.6rem; border-radius:0.5rem; font-size:0.85rem;">${String.fromCharCode(65 + idx)}</span>
                        <span>${opt}</span>
                    </span>
                    <span style="font-size:1.25rem; font-weight:900;">${iconMarker}</span>
                `;
                optionsContainer.appendChild(btn);
            });

            if (answered && gameMode === 'instant') {
                showFeedback(userAnswers[currentIdx] === q.correct, q.explanation);
            }

            document.getElementById('prev-btn').disabled = currentIdx === 0;
            const nextBtn = document.getElementById('next-btn');
            if (currentIdx === questions.length - 1) {
                nextBtn.innerText = "FINISH GAME 🏁";
                nextBtn.className = "btn-quizizz-green font-heading";
            } else {
                nextBtn.innerText = "Selanjutnya →";
                nextBtn.className = "btn-quizizz-purple font-heading";
            }
        }

        function handleOptionClick(selectedIdx) {
            if (userAnswers[currentIdx] !== null && gameMode === 'instant') return;

            const q = questions[currentIdx];
            const isCorrect = selectedIdx === q.correct;
            userAnswers[currentIdx] = selectedIdx;

            if (isCorrect) {
                playSound('correct');
                currentStreak++;
                if (currentStreak > maxStreak) maxStreak = currentStreak;
                const streakBonus = Math.min(currentStreak * 10, 50);
                score += (100 / questions.length) + streakBonus;
                if (currentStreak >= 3) triggerConfetti();
            } else {
                playSound('wrong');
                currentStreak = 0;
            }

            if (!isCorrect && gameMode === 'instant') {
                const app = document.getElementById('app');
                app.classList.add('animate-shake');
                setTimeout(() => app.classList.remove('animate-shake'), 400);
            }

            renderQuestion();
        }

        function showFeedback(isCorrect, explanation) {
            const banner = document.getElementById('feedback-banner');
            const icon = document.getElementById('feedback-icon');
            const title = document.getElementById('feedback-title');
            const text = document.getElementById('feedback-text');

            banner.classList.remove('hidden');

            if (isCorrect) {
                banner.style.borderColor = "rgba(16,185,129,0.5)";
                banner.style.background = "rgba(6,78,59,0.8)";
                banner.style.color = "#a7f3d0";
                icon.innerText = "🎉";
                title.innerText = "JAWABAN BENAR!";
                title.style.color = "#34d399";
            } else {
                banner.style.borderColor = "rgba(244,63,94,0.5)";
                banner.style.background = "rgba(136,19,55,0.8)";
                banner.style.color = "#fecdd3";
                icon.innerText = "💡";
                title.innerText = "JAWABAN KURANG TEPAT";
                title.style.color = "#fb7185";
            }
            text.innerText = explanation;
        }

        function nextQuestion() {
            playSound('pop');
            if (currentIdx < questions.length - 1) {
                currentIdx++;
                renderQuestion();
            } else {
                finishQuiz();
            }
        }

        function prevQuestion() {
            playSound('pop');
            if (currentIdx > 0) {
                currentIdx--;
                renderQuestion();
            }
        }

        function finishQuiz() {
            clearInterval(timerInterval);
            playSound('finish');
            triggerConfetti();

            let correctCount = 0;
            userAnswers.forEach((ans, idx) => {
                if (ans === questions[idx].correct) correctCount++;
            });

            const accuracy = Math.round((correctCount / questions.length) * 100);
            const finalScoreVal = Math.round((correctCount / questions.length) * 100);

            document.getElementById('quiz-screen').classList.add('hidden');
            document.getElementById('quiz-screen').classList.remove('flex');
            document.getElementById('result-screen').classList.remove('hidden');
            document.getElementById('result-screen').classList.add('flex');

            document.getElementById('final-score').innerText = finalScoreVal;
            document.getElementById('final-accuracy').innerText = `${accuracy}%`;
            document.getElementById('max-streak-display').innerText = `${maxStreak} 🔥`;

            const resultEmoji = document.getElementById('result-emoji');
            const resultTitle = document.getElementById('result-title');
            
            if (accuracy >= 80) {
                resultEmoji.innerText = "👑";
                resultTitle.innerText = "LUAR BIASA! MASTER TKA!";
            } else if (accuracy >= 60) {
                resultEmoji.innerText = "⚡";
                resultTitle.innerText = "KEREN! HASIL MEMUASKAN!";
            } else {
                resultEmoji.innerText = "💪";
                resultTitle.innerText = "TETAP SEMANGAT! AYO LATIHAN LAGI!";
            }
        }

        function showReview() {
            playSound('pop');
            document.getElementById('result-screen').classList.add('hidden');
            document.getElementById('result-screen').classList.remove('flex');
            document.getElementById('review-screen').classList.remove('hidden');
            document.getElementById('review-screen').classList.add('flex');

            const reviewList = document.getElementById('review-list');
            reviewList.innerHTML = '';

            questions.forEach((q, idx) => {
                const userAns = userAnswers[idx];
                const isCorrect = userAns === q.correct;

                const card = document.createElement('div');
                card.style.padding = "1rem";
                card.style.borderRadius = "1rem";
                card.style.border = "2px solid";
                card.style.borderColor = isCorrect ? "rgba(16,185,129,0.4)" : "rgba(244,63,94,0.4)";
                card.style.background = isCorrect ? "rgba(6,78,59,0.2)" : "rgba(136,19,55,0.2)";

                let optionsListHtml = '';
                q.options.forEach((opt, oIdx) => {
                    let style = "color: #94a3b8;";
                    let badge = "";

                    if (oIdx === q.correct) {
                        style = "color: #34d399; font-weight: bold;";
                        badge = " <span style='font-size:0.65rem; background:rgba(16,185,129,0.2); color:#6ee7b7; padding:0.1rem 0.5rem; border-radius:9999px; border:1px solid rgba(16,185,129,0.3);'>Kunci Jawaban</span>";
                    }
                    if (oIdx === userAns && !isCorrect) {
                        style = "color: #fb7185; font-weight: bold; text-decoration: line-through;";
                        badge = " <span style='font-size:0.65rem; background:rgba(244,63,94,0.2); color:#fca5a5; padding:0.1rem 0.5rem; border-radius:9999px; border:1px solid rgba(244,63,94,0.3);'>Pilihanmu</span>";
                    } else if (oIdx === userAns && isCorrect) {
                        badge += " <span style='font-size:0.65rem; background:rgba(16,185,129,0.2); color:#6ee7b7; padding:0.1rem 0.5rem; border-radius:9999px; border:1px solid rgba(16,185,129,0.3);'>Pilihanmu</span>";
                    }

                    optionsListHtml += `<li style="${style} font-size: 0.85rem; padding: 0.25rem 0; display: flex; justify-content: space-between; align-items: center;">
                        <span><strong>${String.fromCharCode(65 + oIdx)}.</strong> ${opt}</span>
                        <span>${badge}</span>
                    </li>`;
                });

                card.innerHTML = `
                    <div style="display: flex; justify-content: space-between; align-items: start; margin-bottom: 0.5rem;">
                        <span class="font-heading" style="font-size: 0.75rem; font-weight: 700; color: #c084fc;">SOAL ${idx + 1}</span>
                        <span style="font-size: 0.75rem; font-weight: 900; padding: 0.2rem 0.6rem; border-radius: 9999px; background: ${isCorrect ? 'rgba(16,185,129,0.2)' : 'rgba(244,63,94,0.2)'}; color: ${isCorrect ? '#34d399' : '#fb7185'}; border: 1px solid ${isCorrect ? 'rgba(16,185,129,0.4)' : 'rgba(244,63,94,0.4)'};">
                            ${isCorrect ? 'BENAR' : 'SALAH'}
                        </span>
                    </div>
                    <p style="font-weight: 600; color: #fff; font-size: 0.95rem; margin-bottom: 0.75rem;">${q.question}</p>
                    <ul style="margin-bottom: 0.75rem; background: rgba(15,23,42,0.8); padding: 0.75rem; border-radius: 0.75rem; list-style: none;">${optionsListHtml}</ul>
                    <div style="background: rgba(2,6,23,0.8); padding: 0.75rem; border-radius: 0.75rem; border: 1px solid #1e293b; font-size: 0.8rem; color: #cbd5e1;">
                        <strong style="color: #fbbf24;">💡 Pembahasan:</strong> ${q.explanation}
                    </div>
                `;

                reviewList.appendChild(card);
            });
        }

        function backToResult() {
            playSound('pop');
            document.getElementById('review-screen').classList.add('hidden');
            document.getElementById('review-screen').classList.remove('flex');
            document.getElementById('result-screen').classList.remove('hidden');
            document.getElementById('result-screen').classList.add('flex');
        }

        function restartQuiz() {
            playSound('pop');
            currentIdx = 0;
            score = 0;
            currentStreak = 0;
            maxStreak = 0;
            userAnswers = new Array(questions.length).fill(null);
            secondsElapsed = 0;

            document.getElementById('result-screen').classList.add('hidden');
            document.getElementById('result-screen').classList.remove('flex');
            document.getElementById('welcome-screen').classList.remove('hidden');
        }
    </script>
</body>
</html>

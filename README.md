<!DOCTYPE html>  
<html lang="en">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>SHV.TEST AI — CBSE Class 10 Tutor & Mock Papers</title>  
    <script src="https://cdn.tailwindcss.com"></script>  
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">  
    <!-- Marked.js for Markdown parsing -->  
    <script src="https://cdn.jsdelivr.net/npm/marked/marked.min.js"></script>  
    <!-- MathJax for rendering math equations -->  
    <script>  
        MathJax = {  
            tex: {  
                inlineMath: [['$', '$'], ['\', '\']],  
                displayMath: [['$$', '$$'], ['\', '\']],  
                processEscapes: true  
            },  
            svg: { fontCache: 'global' }  
        };  
    </script>  
    <script type="text/javascript" id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-svg.js"></script>  
      
    <style>  
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');  
          
        body {  
            font-family: 'Inter', sans-serif;  
            background-color: #f3f4f6;  
            color: #1f2937;  
        }  
  
        /* Custom Scrollbar */  
        ::-webkit-scrollbar {  
            width: 8px;  
            height: 8px;  
        }  
        ::-webkit-scrollbar-track {  
            background: #f1f1f1;  
        }  
        ::-webkit-scrollbar-thumb {  
            background: #cbd5e1;  
            border-radius: 4px;  
        }  
        ::-webkit-scrollbar-thumb:hover {  
            background: #94a3b8;  
        }  
  
        /* Markdown Styles in Chat */  
        .markdown-body p { margin-bottom: 0.75em; }  
        .markdown-body p:last-child { margin-bottom: 0; }  
        .markdown-body ul { list-style-type: disc; padding-left: 1.5em; margin-bottom: 0.75em; }  
        .markdown-body ol { list-style-type: decimal; padding-left: 1.5em; margin-bottom: 0.75em; }  
        .markdown-body strong { font-weight: 600; color: #111827; }  
        .markdown-body em { font-style: italic; }  
        .markdown-body code { background-color: rgba(0,0,0,0.1); padding: 0.1em 0.3em; border-radius: 4px; font-family: monospace; font-size: 0.9em; }  
        .markdown-body pre { background-color: #1e293b; color: #f8fafc; padding: 1em; border-radius: 8px; overflow-x: auto; margin-bottom: 0.75em; }  
        .markdown-body pre code { background-color: transparent; padding: 0; color: inherit; }  
        .markdown-body h1, .markdown-body h2, .markdown-body h3 { font-weight: 700; margin-top: 1em; margin-bottom: 0.5em; }  
        .markdown-body h3 { font-size: 1.1em; }  
  
        /* User message specific overrides for markdown */  
        .user-message .markdown-body strong { color: #ffffff; }  
        .user-message .markdown-body code { background-color: rgba(255,255,255,0.2); }  
  
        /* Loader */  
        .dot-flashing {  
            position: relative;  
            width: 8px;  
            height: 8px;  
            border-radius: 5px;  
            background-color: #6366f1;  
            color: #6366f1;  
            animation: dot-flashing 1s infinite linear alternate;  
            animation-delay: 0.5s;  
        }  
        .dot-flashing::before, .dot-flashing::after {  
            content: '';  
            display: inline-block;  
            position: absolute;  
            top: 0;  
        }  
        .dot-flashing::before {  
            left: -12px;  
            width: 8px;  
            height: 8px;  
            border-radius: 5px;  
            background-color: #6366f1;  
            color: #6366f1;  
            animation: dot-flashing 1s infinite alternate;  
            animation-delay: 0s;  
        }  
        .dot-flashing::after {  
            left: 12px;  
            width: 8px;  
            height: 8px;  
            border-radius: 5px;  
            background-color: #6366f1;  
            color: #6366f1;  
            animation: dot-flashing 1s infinite alternate;  
            animation-delay: 1s;  
        }  
        @keyframes dot-flashing {  
            0% { background-color: #6366f1; }  
            50%, 100% { background-color: rgba(99, 102, 241, 0.2); }  
        }  
  
        .glass-panel {  
            background: rgba(255, 255, 255, 0.95);  
            backdrop-filter: blur(10px);  
            border: 1px solid rgba(255, 255, 255, 0.2);  
        }  
          
        .quiz-option {  
            transition: all 0.2s ease;  
        }  
        .quiz-option:hover:not(:disabled) {  
            border-color: #6366f1;  
            background-color: #eff6ff;  
        }  
        .quiz-option.selected {  
            border-color: #6366f1;  
            background-color: #e0e7ff;  
            ring: 2px solid #6366f1;  
        }  
        .quiz-option.correct {  
            border-color: #22c55e;  
            background-color: #f0fdf4;  
            color: #166534;  
        }  
        .quiz-option.incorrect {  
            border-color: #ef4444;  
            background-color: #fef2f2;  
            color: #991b1b;  
        }  
    </style>  
</head>  
<body class="h-screen flex flex-col md:flex-row overflow-hidden">  
  
    <!-- Sidebar -->  
    <nav class="w-full md:w-64 bg-indigo-900 text-white flex flex-col justify-between shadow-xl z-20 shrink-0">  
        <div>  
            <div class="p-6 flex items-center gap-3 border-b border-indigo-800">  
                <div class="w-10 h-10 rounded-full bg-white text-indigo-900 flex items-center justify-center font-bold text-xl shadow-inner">  
                    <i class="fa-solid fa-graduation-cap"></i>  
                </div>  
                <div>  
                    <h1 class="text-xl font-bold tracking-wide">SHV.TEST</h1>  
                    <p class="text-indigo-300 text-xs tracking-wider">AI TUTOR CLASS 10</p>  
                </div>  
            </div>  
            <div class="p-4 space-y-2 overflow-y-auto max-h-[calc(100vh-140px)]">  
                <button onclick="switchTab('tutor')" id="tab-tutor" class="w-full text-left px-4 py-3 rounded-xl transition-all duration-200 bg-indigo-700 font-medium flex items-center gap-3 shadow-md">  
                    <i class="fa-solid fa-chalkboard-user w-5 text-center"></i> AI Tutor  
                </button>  
                <button onclick="switchTab('generator')" id="tab-generator" class="w-full text-left px-4 py-3 rounded-xl transition-all duration-200 hover:bg-indigo-800 text-indigo-100 flex items-center gap-3">  
                    <i class="fa-solid fa-file-signature w-5 text-center"></i> Question Generator  
                </button>  
                <button onclick="switchTab('brainstorm')" id="tab-brainstorm" class="w-full text-left px-4 py-3 rounded-xl transition-all duration-200 hover:bg-indigo-800 text-indigo-100 flex items-center gap-3">  
                    <i class="fa-solid fa-brain w-5 text-center"></i> Brainstorm Arena (HOTS)  
                </button>  
                <button onclick="switchTab('mockpaper')" id="tab-mockpaper" class="w-full text-left px-4 py-3 rounded-xl transition-all duration-200 hover:bg-indigo-800 text-indigo-100 flex items-center gap-3">  
                    <i class="fa-solid fa-file-lines w-5 text-center"></i> 80-Marks Mock Paper  
                </button>  
                <button onclick="switchTab('mistakes')" id="tab-mistakes" class="w-full text-left px-4 py-3 rounded-xl transition-all duration-200 hover:bg-indigo-800 text-indigo-100 flex items-center gap-3">  
                    <i class="fa-solid fa-book-open w-5 text-center"></i> Mistake Notebook  
                </button>  
                <button onclick="switchTab('progress')" id="tab-progress" class="w-full text-left px-4 py-3 rounded-xl transition-all duration-200 hover:bg-indigo-800 text-indigo-100 flex items-center gap-3">  
                    <i class="fa-solid fa-chart-line w-5 text-center"></i> Progress Tracker  
                </button>  
            </div>  
        </div>  
        <div class="p-4 border-t border-indigo-800 text-sm text-indigo-300 text-center hidden md:block">  
            CBSE NCERT Aligned Mode  
        </div>  
    </nav>  
  
    <!-- Main Content Area -->  
    <main class="flex-1 relative flex flex-col h-full bg-gray-50 overflow-hidden">  
          
        <!-- Toast Notification Container -->  
        <div id="toast-container" class="absolute top-4 left-1/2 transform -translate-x-1/2 z-50 flex flex-col gap-2 pointer-events-none"></div>  
  
        <!-- APP: AI TUTOR MODE -->  
        <div id="view-tutor" class="flex-1 flex flex-col h-full w-full absolute inset-0 transition-opacity duration-300">  
            <!-- Header -->  
            <header class="glass-panel p-4 shadow-sm flex items-center justify-between z-10 shrink-0">  
                <div>  
                    <h2 class="text-lg font-bold text-gray-800 flex items-center gap-2">  
                        <i class="fa-solid fa-robot text-indigo-600"></i> Personal AI Tutor  
                    </h2>  
                    <p class="text-sm text-gray-500">Ask any Class 10 doubt (Hinglish/English)</p>  
                </div>  
                <button onclick="clearChat()" class="text-gray-400 hover:text-red-500 transition-colors p-2" title="Clear Chat">  
                    <i class="fa-solid fa-trash-can"></i>  
                </button>  
            </header>  
  
            <!-- Chat Messages -->  
            <div id="chat-container" class="flex-1 overflow-y-auto p-4 md:p-6 space-y-6 scroll-smooth pb-32">  
                <!-- Welcome Message -->  
                <div class="flex gap-4">  
                    <div class="w-10 h-10 rounded-full bg-indigo-100 text-indigo-600 flex items-center justify-center shrink-0">  
                        <i class="fa-solid fa-robot"></i>  
                    </div>  
                    <div class="bg-white p-4 rounded-2xl rounded-tl-none shadow-sm border border-gray-100 max-w-[85%] text-gray-800">  
                        <p class="font-medium mb-1">Namaste! 👋</p>  
                        <p>I am your Class 10 CBSE AI Tutor. I can help you with Maths, Science, Social Science, and English.</p>  
                        <p class="mt-2 text-sm text-gray-600">What would you like to study today? (Aap kya padhna chahenge?)</p>  
                    </div>  
                </div>  
            </div>  
  
            <!-- Typing Indicator (Hidden by default) -->  
            <div id="typing-indicator" class="hidden absolute bottom-24 left-6 md:left-8 flex gap-4">  
                 <div class="w-10 h-10 rounded-full bg-indigo-100 text-indigo-600 flex items-center justify-center shrink-0">  
                    <i class="fa-solid fa-robot"></i>  
                </div>  
                <div class="bg-white p-4 rounded-2xl rounded-tl-none shadow-sm border border-gray-100 flex items-center justify-center min-w-[80px]">  
                    <div class="dot-flashing"></div>  
                </div>  
            </div>  
  
            <!-- Input Area -->  
            <div class="glass-panel p-4 absolute bottom-0 w-full border-t border-gray-200 z-10">  
                <form id="chat-form" class="max-w-5xl mx-auto relative flex items-end gap-2">  
                    <textarea   
                        id="chat-input"   
                        class="w-full bg-white border border-gray-300 rounded-2xl pl-4 pr-12 py-3 focus:outline-none focus:ring-2 focus:ring-indigo-500 focus:border-transparent resize-none h-14"   
                        placeholder="Type your question here... e.g. Explain Ohm's Law"  
                        rows="1"  
                        oninput="this.style.height = '';this.style.height = Math.min(this.scrollHeight, 120) + 'px'"  
                        onkeydown="if(event.key === 'Enter' && !event.shiftKey) { event.preventDefault(); document.getElementById('chat-form').dispatchEvent(new Event('submit')); }"  
                    ></textarea>  
                    <button type="submit" class="bg-indigo-600 hover:bg-indigo-700 text-white w-12 h-12 rounded-full flex items-center justify-center transition-colors shadow-md shrink-0 absolute right-1 bottom-1">  
                        <i class="fa-solid fa-paper-plane"></i>  
                    </button>  
                </form>  
                <div class="text-center mt-2 text-xs text-gray-400">Powered by Gemini AI. Verify board-critical information with NCERT.</div>  
            </div>  
        </div>  
  
        <!-- APP: QUESTION GENERATOR MODE -->  
        <div id="view-generator" class="flex-1 flex flex-col h-full w-full absolute inset-0 opacity-0 pointer-events-none transition-opacity duration-300 bg-white">  
              
            <header class="glass-panel p-4 shadow-sm border-b border-gray-200 z-10 shrink-0">  
                <h2 class="text-lg font-bold text-gray-800 flex items-center gap-2">  
                    <i class="fa-solid fa-file-signature text-indigo-600"></i> Question Generator  
                </h2>  
                <p class="text-sm text-gray-500">Generate targeted practice questions (5 to 30 questions)</p>  
            </header>  
  
            <div class="flex-1 overflow-y-auto p-4 md:p-6">  
                <!-- Configuration Form -->  
                <div id="generator-setup" class="max-w-4xl mx-auto bg-white rounded-2xl shadow-lg border border-gray-100 p-6">  
                    <h3 class="text-xl font-bold mb-6 text-gray-800 border-b pb-2">Test Setup</h3>  
                      
                    <form id="generator-form" class="space-y-6">  
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">  
                            <!-- Subject -->  
                            <div>  
                                <label class="block text-sm font-semibold text-gray-700 mb-2">Subject</label>  
                                <select id="gen-subject" class="w-full p-3 bg-gray-50 border border-gray-300 rounded-xl focus:ring-2 focus:ring-indigo-500 focus:outline-none" required onchange="updateChapters()">  
                                    <option value="" disabled selected>Select Subject</option>  
                                    <option value="Mathematics">Mathematics</option>  
                                    <option value="Science">Science</option>  
                                    <option value="Social Science">Social Science</option>  
                                    <option value="English">English</option>  
                                </select>  
                            </div>  
                            <!-- Chapter -->  
                            <div>  
                                <label class="block text-sm font-semibold text-gray-700 mb-2">Chapter</label>  
                                <select id="gen-chapter" class="w-full p-3 bg-gray-50 border border-gray-300 rounded-xl focus:ring-2 focus:ring-indigo-500 focus:outline-none" required disabled>  
                                    <option value="" disabled selected>Select Subject First</option>  
                                </select>  
                            </div>  
                            <!-- Format -->  
                            <div>  
                                <label class="block text-sm font-semibold text-gray-700 mb-2">Format</label>  
                                <select id="gen-format" class="w-full p-3 bg-gray-50 border border-gray-300 rounded-xl focus:ring-2 focus:ring-indigo-500 focus:outline-none" required>  
                                    <option value="MCQ">Multiple Choice (MCQ)</option>  
                                    <option value="Assertion-Reason">Assertion-Reason</option>  
                                    <option value="Case Study">Case Study Based</option>  
                                    <option value="Competency Based">Competency Based</option>  
                                    <option value="Mixed">Mixed Formats</option>  
                                </select>  
                            </div>  
                            <!-- Difficulty -->  
                            <div>  
                                <label class="block text-sm font-semibold text-gray-700 mb-2">Difficulty Level</label>  
                                <select id="gen-difficulty" class="w-full p-3 bg-gray-50 border border-gray-300 rounded-xl focus:ring-2 focus:ring-indigo-500 focus:outline-none" required>  
                                    <option value="Medium">Medium (Standard)</option>  
                                    <option value="Easy">Easy (Basic Concepts)</option>  
                                    <option value="HOTS">HOTS (Higher Order Thinking)</option>  
                                    <option value="Full Board Level">Full Board Level (Exam Style)</option>  
                                </select>  
                            </div>  
                            <!-- Count (5 to 30) -->  
                            <div>  
                                <label class="block text-sm font-semibold text-gray-700 mb-2">Number of Questions (5 to 30)</label>  
                                <div class="flex items-center gap-4">  
                                    <input type="range" id="gen-count-range" min="5" max="30" value="10" class="w-full accent-indigo-600" oninput="document.getElementById('gen-count').value = this.value">  
                                    <input type="number" id="gen-count" min="5" max="30" value="10" class="w-24 p-3 bg-gray-50 border border-gray-300 rounded-xl text-center font-bold focus:ring-2 focus:ring-indigo-500 focus:outline-none" oninput="document.getElementById('gen-count-range').value = this.value" required>  
                                </div>  
                            </div>  
                            <!-- Timer Toggle (Mann pe h) -->  
                            <div class="flex items-center justify-between p-4 bg-gray-50 rounded-xl border border-gray-200">  
                                <div>  
                                    <label class="block text-sm font-semibold text-gray-700 cursor-pointer" for="gen-timer-toggle">Enable Quiz Timer</label>  
                                    <p class="text-xs text-gray-500">Optional countdown timer for practice</p>  
                                </div>  
                                <input type="checkbox" id="gen-timer-toggle" class="w-5 h-5 text-indigo-600 rounded focus:ring-indigo-500 accent-indigo-600 cursor-pointer">  
                            </div>  
                        </div>  
  
                        <div class="pt-4 flex justify-end">  
                            <button type="submit" id="btn-generate" class="bg-indigo-600 hover:bg-indigo-700 text-white font-bold py-3 px-8 rounded-xl shadow-lg transition-all transform hover:-translate-y-0.5 flex items-center gap-2">  
                                <i class="fa-solid fa-wand-magic-sparkles"></i> Generate Questions  
                            </button>  
                        </div>  
                    </form>  
                </div>  
  
                <!-- Generation Loading State -->  
                <div id="generator-loading" class="hidden flex-col items-center justify-center py-20">  
                    <i class="fa-solid fa-microchip text-4xl text-indigo-500 animate-pulse mb-4"></i>  
                    <h3 class="text-xl font-bold text-gray-800">Generating Assessment...</h3>  
                    <p class="text-gray-500 mt-2 text-center max-w-md">Crafting high-quality CBSE Class 10 aligned questions based on your strict criteria. This takes about 5-10 seconds.</p>  
                </div>  
  
                <!-- Quiz Interface -->  
                <div id="quiz-container" class="hidden max-w-4xl mx-auto space-y-6 pb-20">  
                    <!-- Quiz Header & Timer -->  
                    <div class="flex flex-col md:flex-row justify-between items-start md:items-center border-b pb-4 mt-4 gap-4">  
                        <div id="quiz-header"></div>  
                        <div id="quiz-timer-display" class="hidden bg-indigo-50 border border-indigo-200 text-indigo-900 px-4 py-2 rounded-xl font-bold flex items-center gap-2 shadow-sm">  
                            <i class="fa-solid fa-stopwatch text-indigo-600"></i> <span id="timer-c
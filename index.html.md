**<!DOCTYPE html>**

**<html lang="ar" dir="rtl">**

**<head>**

&#x20;   **<meta charset="UTF-8">**

&#x20;   **<meta name="viewport" content="width=device-width, initial-scale=1.0">**

&#x20;   **<title>خُطى للرعاية الصحية - دانة المطيري</title>**

&#x20;   

&#x20;   **<link rel="preconnect" href="https://fonts.googleapis.com">**

&#x20;   **<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>**

&#x20;   **<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;600;700;900\&display=swap" rel="stylesheet">**

&#x20;   **<script src="https://cdn.tailwindcss.com"></script>**

&#x20;   **<script src="https://unpkg.com/lucide@latest"></script>**



&#x20;   **<script>**

&#x20;       **tailwind.config = {**

&#x20;           **theme: {**

&#x20;               **extend: {**

&#x20;                   **fontFamily: { sans: \['Cairo', 'sans-serif'] },**

&#x20;                   **colors: {**

&#x20;                       **medical: {**

&#x20;                           **50: '#f0fdf4',**

&#x20;                           **100: '#dcfce7',**

&#x20;                           **500: '#10b981',** 

&#x20;                           **600: '#059669',**

&#x20;                           **700: '#047857',**

&#x20;                           **blue: '#0ea5e9',**

&#x20;                           **darkBlue: '#0369a1',**

&#x20;                       **}**

&#x20;                   **},**

&#x20;                   **backgroundImage: {**

&#x20;                       **'gradient-medical': 'linear-gradient(135deg, #0ea5e9 0%, #10b981 100%)',**

&#x20;                   **}**

&#x20;               **}**

&#x20;           **}**

&#x20;       **}**

&#x20;   **</script>**



&#x20;   **<style>**

&#x20;       **body {**

&#x20;           **background-color: #f8fafc;**

&#x20;           **background-image: linear-gradient(135deg, rgba(255, 255, 255, 0.9) 0%, rgba(240, 253, 244, 0.9) 100%),** 

&#x20;                             **url('https://images.unsplash.com/photo-1516549655169-df83a0774514?auto=format\&fit=crop\&q=80\&w=2000');**

&#x20;           **background-attachment: fixed;**

&#x20;           **background-size: cover;**

&#x20;           **scroll-behavior: smooth;**

&#x20;       **}**

&#x20;       **.page-section { display: none; opacity: 0; transform: translateY(20px); transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1); }**

&#x20;       **.page-section.active { display: block; opacity: 1; transform: translateY(0); }**

&#x20;       

&#x20;       **.glass-card {**

&#x20;           **background: rgba(255, 255, 255, 0.85);**

&#x20;           **backdrop-filter: blur(12px);**

&#x20;           **border: 1px solid rgba(255, 255, 255, 0.5);**

&#x20;           **transition: all 0.3s ease;**

&#x20;       **}**

&#x20;       **.glass-card:hover {**

&#x20;           **transform: translateY(-5px);**

&#x20;           **box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.05);**

&#x20;       **}**

&#x20;       **.nav-btn.active-link {**

&#x20;           **color: #059669;**

&#x20;           **border-bottom: 2px solid #059669;**

&#x20;       **}**

&#x20;       **.bg-mix {**

&#x20;           **background: linear-gradient(135deg, #0ea5e9 0%, #10b981 100%);**

&#x20;       **}**

&#x20;       **.text-gradient {**

&#x20;           **background: linear-gradient(135deg, #0369a1 0%, #047857 100%);**

&#x20;           **-webkit-background-clip: text;**

&#x20;           **-webkit-text-fill-color: transparent;**

&#x20;       **}**

&#x20;       **@keyframes float {**

&#x20;           **0% { transform: translateY(0px); }**

&#x20;           **50% { transform: translateY(-10px); }**

&#x20;           **100% { transform: translateY(0px); }**

&#x20;       **}**

&#x20;       **.float-anim { animation: float 3s ease-in-out infinite; }**

&#x20;   **</style>**

**</head>**

**<body class="font-sans min-h-screen flex flex-col text-slate-800">**



&#x20;   **<!-- Navigation -->**

&#x20;   **<nav class="bg-white/90 backdrop-blur-md shadow-sm sticky top-0 z-50 border-b border-emerald-50">**

&#x20;       **<div class="container mx-auto px-4 py-3 flex justify-between items-center">**

&#x20;           **<div class="flex items-center gap-3 cursor-pointer group" onclick="showPage('home')">**

&#x20;               **<div class="w-12 h-12 bg-mix rounded-xl shadow-lg flex items-center justify-center transition-transform group-hover:rotate-12">**

&#x20;                   **<svg width="32" height="32" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-white">**

&#x20;                       **<path d="M3 12H7L9 5L12 19L15 9L17 12H21" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"/>**

&#x20;                   **</svg>**

&#x20;               **</div>**

&#x20;               **<span class="text-2xl font-black text-gradient tracking-tight">خُـطـى</span>**

&#x20;           **</div>**

&#x20;           **<div class="hidden lg:flex gap-8 text-sm font-bold text-slate-600">**

&#x20;               **<button onclick="showPage('home')" class="nav-btn hover:text-medical-600 transition pb-1 active-link">الرئيسية</button>**

&#x20;               **<button onclick="showPage('bot')" class="nav-btn hover:text-medical-600 transition pb-1">المساعد الذكي</button>**

&#x20;               **<button onclick="showPage('analysis')" class="nav-btn hover:text-medical-600 transition pb-1">تحليل التقارير</button>**

&#x20;               **<button onclick="showPage('tracker')" class="nav-btn hover:text-medical-600 transition pb-1">تتبع الصحة</button>**

&#x20;           **</div>**

&#x20;           **<div class="flex items-center gap-4">**

&#x20;                **<button onclick="showPage('emergency')" class="bg-red-600 text-white px-5 py-2 rounded-xl font-bold flex items-center gap-2 hover:bg-red-700 transition shadow-lg shadow-red-100">**

&#x20;                   **<i data-lucide="phone-forwarded" class="w-4 h-4"></i> طوارئ**

&#x20;               **</button>**

&#x20;           **</div>**

&#x20;       **</div>**

&#x20;   **</nav>**



&#x20;   **<main class="flex-grow container mx-auto px-4 py-10 max-w-6xl">**



&#x20;       **<!-- Home Page -->**

&#x20;       **<section id="home" class="page-section active">**

&#x20;           **<!-- Hero -->**

&#x20;           **<div class="flex flex-col items-center text-center space-y-8 mb-20">**

&#x20;               **<div class="relative float-anim">**

&#x20;                   **<div class="absolute inset-0 bg-medical-500 blur-3xl opacity-20 rounded-full animate-pulse"></div>**

&#x20;                   **<div class="w-48 h-48 md:w-64 md:h-64 bg-white rounded-\[3rem] shadow-2xl relative z-10 flex items-center justify-center border-8 border-white p-6">**

&#x20;                       **<svg viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg" class="w-full h-full">**

&#x20;                           **<defs>**

&#x20;                               **<linearGradient id="logoGrad" x1="0%" y1="0%" x2="100%" y2="100%">**

&#x20;                                   **<stop offset="0%" style="stop-color:#0ea5e9;stop-opacity:1" />**

&#x20;                                   **<stop offset="100%" style="stop-color:#10b981;stop-opacity:1" />**

&#x20;                               **</linearGradient>**

&#x20;                           **</defs>**

&#x20;                           **<rect width="100" height="100" rx="30" fill="#f0fdf4"/>**

&#x20;                           **<path d="M20 50H35L45 20L55 80L65 40L75 50H85" stroke="url(#logoGrad)" stroke-width="6" stroke-linecap="round" stroke-linejoin="round"/>**

&#x20;                       **</svg>**

&#x20;                   **</div>**

&#x20;               **</div>**

&#x20;               

&#x20;               **<h1 class="text-5xl md:text-7xl font-black text-slate-900 leading-tight">**

&#x20;                   **<span class="text-gradient">خُـطـى</span> نحو مستقبل آمن**

&#x20;               **</h1>**

&#x20;               **<p class="text-xl text-slate-500 max-w-3xl mx-auto leading-relaxed font-medium">**

&#x20;                   **تقنيات الذكاء الاصطناعي بين يديك. مزيج من <span class="text-medical-blue font-bold">الابتكار الرقمي</span> و <span class="text-medical-500 font-bold">الرعاية الإنسانية</span> لرسم ملامح صحتك.**

&#x20;               **</p>**

&#x20;               

&#x20;               **<div class="flex flex-wrap justify-center gap-4 pt-4">**

&#x20;                   **<button onclick="showPage('bot')" class="bg-mix text-white px-10 py-4 rounded-2xl font-bold shadow-2xl hover:shadow-emerald-200 transition transform hover:-translate-y-1">**

&#x20;                       **تحدث مع المساعد الذكي**

&#x20;                   **</button>**

&#x20;                   **<button onclick="showPage('analysis')" class="bg-white text-medical-700 border-2 border-emerald-100 px-10 py-4 rounded-2xl font-bold shadow-sm hover:bg-emerald-50 transition">**

&#x20;                       **قراءة تقرير طبي**

&#x20;                   **</button>**

&#x20;               **</div>**

&#x20;           **</div>**



&#x20;           **<!-- Stats Bar (New Addition) -->**

&#x20;           **<div class="grid grid-cols-2 md:grid-cols-4 gap-4 mb-20">**

&#x20;               **<div class="glass-card p-6 rounded-3xl text-center">**

&#x20;                   **<p class="text-3xl font-black text-medical-600">+150K</p>**

&#x20;                   **<p class="text-xs text-slate-400 font-bold uppercase mt-1">استشارة ذكية</p>**

&#x20;               **</div>**

&#x20;               **<div class="glass-card p-6 rounded-3xl text-center">**

&#x20;                   **<p class="text-3xl font-black text-medical-blue">99.2%</p>**

&#x20;                   **<p class="text-xs text-slate-400 font-bold uppercase mt-1">دقة التحليل</p>**

&#x20;               **</div>**

&#x20;               **<div class="glass-card p-6 rounded-3xl text-center">**

&#x20;                   **<p class="text-3xl font-black text-medical-600">24/7</p>**

&#x20;                   **<p class="text-xs text-slate-400 font-bold uppercase mt-1">دعم طبي فوري</p>**

&#x20;               **</div>**

&#x20;               **<div class="glass-card p-6 rounded-3xl text-center">**

&#x20;                   **<p class="text-3xl font-black text-medical-blue">+50</p>**

&#x20;                   **<p class="text-xs text-slate-400 font-bold uppercase mt-1">طبيب خبير</p>**

&#x20;               **</div>**

&#x20;           **</div>**



&#x20;           **<!-- Features Cards -->**

&#x20;           **<div class="grid grid-cols-1 md:grid-cols-3 gap-8 mb-20">**

&#x20;               **<div class="glass-card p-8 rounded-\[2.5rem] shadow-xl text-center cursor-pointer hover:bg-white transition group" onclick="showPage('bot')">**

&#x20;                   **<div class="w-16 h-16 bg-sky-50 text-sky-600 rounded-2xl flex items-center justify-center mx-auto mb-6 group-hover:bg-sky-500 group-hover:text-white transition-colors">**

&#x20;                       **<i data-lucide="bot" size="32"></i>**

&#x20;                   **</div>**

&#x20;                   **<h3 class="font-bold text-xl mb-3">تشخيص فوري</h3>**

&#x20;                   **<p class="text-slate-500 text-sm">تحليل فائق السرعة للأعراض وتوجيه للمسار الطبي الصحيح عبر مساعدنا الذكي.</p>**

&#x20;               **</div>**

&#x20;               **<div class="glass-card p-8 rounded-\[2.5rem] shadow-xl text-center cursor-pointer hover:bg-white transition group" onclick="showPage('analysis')">**

&#x20;                   **<div class="w-16 h-16 bg-emerald-50 text-emerald-600 rounded-2xl flex items-center justify-center mx-auto mb-6 group-hover:bg-emerald-500 group-hover:text-white transition-colors">**

&#x20;                       **<i data-lucide="file-text" size="32"></i>**

&#x20;                   **</div>**

&#x20;                   **<h3 class="font-bold text-xl mb-3">تحليل التقارير</h3>**

&#x20;                   **<p class="text-slate-500 text-sm">بياناتك الطبية مشفرة ومحمية بأعلى معايير الأمن الرقمي، ارفع ملفك الآن لفك شفرة نتائجك.</p>**

&#x20;               **</div>**

&#x20;               **<div class="glass-card p-8 rounded-\[2.5rem] shadow-xl text-center cursor-pointer hover:bg-white transition group" onclick="showPage('tracker')">**

&#x20;                   **<div class="w-16 h-16 bg-teal-50 text-teal-600 rounded-2xl flex items-center justify-center mx-auto mb-6 group-hover:bg-teal-500 group-hover:text-white transition-colors">**

&#x20;                       **<i data-lucide="calendar-check" size="32"></i>**

&#x20;                   **</div>**

&#x20;                   **<h3 class="font-bold text-xl mb-3">تتبع الحالة</h3>**

&#x20;                   **<p class="text-slate-500 text-sm">إدارة المواعيد والجرعات الدوائية بشكل آلي ومنظم عبر سجل خُطى الزمني الذكي.</p>**

&#x20;               **</div>**

&#x20;           **</div>**



&#x20;           **<!-- Daily Insight (New Addition) -->**

&#x20;           **<div class="bg-mix rounded-\[3rem] p-8 md:p-12 text-white relative overflow-hidden mb-20">**

&#x20;               **<div class="absolute top-0 right-0 p-10 opacity-10">**

&#x20;                   **<i data-lucide="heart" size="120"></i>**

&#x20;               **</div>**

&#x20;               **<div class="relative z-10 max-w-2xl">**

&#x20;                   **<h3 class="text-2xl font-black mb-4 flex items-center gap-2">**

&#x20;                       **<i data-lucide="sparkles"></i> نصيحة "خُطى" لهذا اليوم**

&#x20;                   **</h3>**

&#x20;                   **<p class="text-lg opacity-90 leading-relaxed">**

&#x20;                       **"الاستمرارية في المشي لمدة 20 دقيقة يومياً تعزز من كفاءة القلب بنسبة 30%. تذكر أن خُطى صغيرة اليوم تصنع فارقاً كبيراً غداً."**

&#x20;                   **</p>**

&#x20;                   **<button class="mt-8 bg-white text-medical-600 px-6 py-3 rounded-xl font-bold hover:bg-opacity-90 transition">**

&#x20;                       **اكتشف المزيد من النصائح**

&#x20;                   **</button>**

&#x20;               **</div>**

&#x20;           **</div>**

&#x20;       **</section>**



&#x20;       **<!-- Chatbot Section -->**

&#x20;       **<section id="bot" class="page-section">**

&#x20;           **<div class="grid grid-cols-1 lg:grid-cols-3 gap-6">**

&#x20;               **<!-- Chat UI -->**

&#x20;               **<div class="lg:col-span-2 bg-white rounded-\[2rem] shadow-2xl border border-emerald-50 overflow-hidden flex flex-col h-\[650px]">**

&#x20;                   **<div class="bg-mix p-6 text-white flex items-center gap-4">**

&#x20;                       **<div class="w-10 h-10 bg-white/20 rounded-lg flex items-center justify-center p-2 backdrop-blur">**

&#x20;                            **<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-white">**

&#x20;                               **<path d="M3 12H7L9 5L12 19L15 9L17 12H21" stroke="currentColor" stroke-width="3" stroke-linecap="round" stroke-linejoin="round"/>**

&#x20;                           **</svg>**

&#x20;                       **</div>**

&#x20;                       **<div>**

&#x20;                           **<h3 class="font-bold text-lg leading-none">مساعد خُطى الذكي</h3>**

&#x20;                           **<span class="text-xs text-blue-50">متصل الآن بنظام الذكاء الهجين</span>**

&#x20;                       **</div>**

&#x20;                   **</div>**

&#x20;                   **<div id="chatHistory" class="flex-grow p-6 overflow-y-auto space-y-4 bg-slate-50/50">**

&#x20;                       **<div class="flex gap-3 text-right">**

&#x20;                           **<div class="w-8 h-8 bg-emerald-100 text-emerald-600 rounded-full flex items-center justify-center flex-shrink-0">**

&#x20;                               **<i data-lucide="bot" size="18"></i>**

&#x20;                           **</div>**

&#x20;                           **<div class="bg-white p-4 rounded-2xl rounded-tr-none shadow-sm border border-emerald-50 max-w-\[85%] text-sm">**

&#x20;                               **مرحباً بك. أنا هنا لمساعدتك. هل تعاني من أعراض معينة تود استشارتي بها؟**

&#x20;                           **</div>**

&#x20;                       **</div>**

&#x20;                   **</div>**

&#x20;                   **<div class="p-4 bg-white border-t flex flex-col gap-3">**

&#x20;                       **<div class="flex gap-2">**

&#x20;                            **<input type="text" id="chatInput" placeholder="اكتب سؤالك هنا..." class="flex-grow px-4 py-3 rounded-xl border border-slate-200 focus:ring-2 focus:ring-emerald-500/20 focus:outline-none">**

&#x20;                           **<button onclick="sendMessage()" class="bg-mix text-white px-6 py-3 rounded-xl font-bold hover:opacity-90 transition">**

&#x20;                               **<i data-lucide="send" size="20"></i>**

&#x20;                           **</button>**

&#x20;                       **</div>**

&#x20;                       **<div class="flex flex-wrap gap-2">**

&#x20;                           **<button onclick="quickAsk('أشعر بصداع')" class="text-\[10px] bg-slate-100 px-3 py-1.5 rounded-full hover:bg-emerald-50 transition font-bold text-slate-600 border">أشعر بصداع</button>**

&#x20;                           **<button onclick="quickAsk('كيف أحجز موعد؟')" class="text-\[10px] bg-slate-100 px-3 py-1.5 rounded-full hover:bg-emerald-50 transition font-bold text-slate-600 border">كيف أحجز موعد؟</button>**

&#x20;                           **<button onclick="quickAsk('نصيحة غذائية')" class="text-\[10px] bg-slate-100 px-3 py-1.5 rounded-full hover:bg-emerald-50 transition font-bold text-slate-600 border">نصيحة غذائية</button>**

&#x20;                       **</div>**

&#x20;                   **</div>**

&#x20;               **</div>**



&#x20;               **<!-- Side Tracker -->**

&#x20;               **<div class="flex flex-col gap-6">**

&#x20;                   **<div class="glass-card rounded-\[2rem] p-6 shadow-xl border-emerald-50">**

&#x20;                       **<h3 class="text-xl font-black mb-4 flex items-center gap-2">**

&#x20;                           **<span class="w-1.5 h-6 bg-mix rounded-full"></span>**

&#x20;                           **مسار الحالة الصحي**

&#x20;                       **</h3>**

&#x20;                       **<div class="space-y-6">**

&#x20;                           **<div class="flex gap-4">**

&#x20;                               **<div class="flex flex-col items-center">**

&#x20;                                   **<div class="w-6 h-6 rounded-full bg-emerald-500 border-4 border-white shadow-sm z-10"></div>**

&#x20;                                   **<div class="w-0.5 h-10 bg-emerald-100 -mt-1"></div>**

&#x20;                               **</div>**

&#x20;                               **<div>**

&#x20;                                   **<p class="text-xs font-bold text-emerald-600">تم تسجيل الدخول</p>**

&#x20;                                   **<p class="text-\[10px] text-slate-400">10:30 صباحاً</p>**

&#x20;                               **</div>**

&#x20;                           **</div>**

&#x20;                           **<div class="flex gap-4">**

&#x20;                               **<div class="flex flex-col items-center">**

&#x20;                                   **<div class="w-6 h-6 rounded-full bg-emerald-500 border-4 border-white shadow-sm z-10 pulse-anim"></div>**

&#x20;                                   **<div class="w-0.5 h-10 bg-slate-100 -mt-1"></div>**

&#x20;                               **</div>**

&#x20;                               **<div>**

&#x20;                                   **<p class="text-xs font-bold text-slate-700">قيد الاستشارة</p>**

&#x20;                                   **<p class="text-\[10px] text-slate-400">المساعد الذكي نشط</p>**

&#x20;                               **</div>**

&#x20;                           **</div>**

&#x20;                           **<div class="flex gap-4">**

&#x20;                               **<div class="flex flex-col items-center">**

&#x20;                                   **<div class="w-6 h-6 rounded-full bg-slate-100 border-4 border-white shadow-sm z-10"></div>**

&#x20;                               **</div>**

&#x20;                               **<div>**

&#x20;                                   **<p class="text-xs font-bold text-slate-300">التوصية النهائية</p>**

&#x20;                                   **<p class="text-\[10px] text-slate-300">لم يكتمل بعد</p>**

&#x20;                               **</div>**

&#x20;                           **</div>**

&#x20;                       **</div>**

&#x20;                   **</div>**

&#x20;                   

&#x20;                   **<div class="glass-card rounded-\[2rem] p-6 shadow-xl border-emerald-50 bg-sky-50/30">**

&#x20;                       **<h4 class="font-bold text-sky-700 flex items-center gap-2 mb-4">**

&#x20;                           **<i data-lucide="info" size="18"></i> تنبيه ذكي**

&#x20;                       **</h4>**

&#x20;                       **<p class="text-xs text-slate-600 leading-relaxed">**

&#x20;                           **تذكر إرفاق صور واضحة للتقارير الطبية في قسم التحليل للحصول على أفضل النتائج.**

&#x20;                       **</p>**

&#x20;                   **</div>**

&#x20;               **</div>**

&#x20;           **</div>**

&#x20;       **</section>**



&#x20;       **<!-- Analysis Section -->**

&#x20;       **<section id="analysis" class="page-section">**

&#x20;           **<div class="max-w-3xl mx-auto">**

&#x20;               **<div class="glass-card rounded-\[2.5rem] p-10 text-center shadow-xl border-emerald-100 mb-8">**

&#x20;                   **<h2 class="text-3xl font-black mb-6 text-medical-700">تحليل التقارير الذكي</h2>**

&#x20;                   **<p class="text-slate-500 mb-8 max-w-md mx-auto">ارفع تقريرك الطبي (PDF أو صورة) وسيقوم الذكاء الاصطناعي بتحليل النتائج وشرح المصطلحات المعقدة لك.</p>**

&#x20;                   

&#x20;                   **<label class="border-2 border-dashed border-emerald-200 rounded-3xl p-12 block cursor-pointer hover:bg-emerald-50/30 transition group mb-6">**

&#x20;                       **<input type="file" id="fileInput" class="hidden" onchange="handleFile(this)">**

&#x20;                       **<div class="w-20 h-20 bg-emerald-50 rounded-full flex items-center justify-center mx-auto mb-4 group-hover:scale-110 transition">**

&#x20;                           **<i data-lucide="upload-cloud" size="40" class="text-emerald-500"></i>**

&#x20;                       **</div>**

&#x20;                       **<p class="text-slate-600 font-bold">اسحب صورة التقرير الطبي أو انقر هنا</p>**

&#x20;                       **<p class="text-slate-400 text-xs mt-2">نحن ندعم الصور، الـ PDF، والتقارير الممسوحة ضوئياً</p>**

&#x20;                   **</label>**



&#x20;                   **<div id="fileResult" class="hidden text-right bg-white p-6 rounded-3xl border border-emerald-100 shadow-sm">**

&#x20;                       **<!-- Content generated by JS -->**

&#x20;                   **</div>**

&#x20;               **</div>**

&#x20;               

&#x20;               **<div class="grid grid-cols-1 md:grid-cols-2 gap-6">**

&#x20;                   **<div class="glass-card p-6 rounded-3xl flex gap-4 items-center">**

&#x20;                       **<div class="w-12 h-12 bg-emerald-100 text-emerald-600 rounded-2xl flex items-center justify-center shrink-0">**

&#x20;                           **<i data-lucide="lock" size="24"></i>**

&#x20;                       **</div>**

&#x20;                       **<div>**

&#x20;                           **<p class="font-bold text-slate-700">خصوصية تامة</p>**

&#x20;                           **<p class="text-xs text-slate-400">تتم معالجة بياناتك محلياً ومشفرة بالكامل.</p>**

&#x20;                       **</div>**

&#x20;                   **</div>**

&#x20;                   **<div class="glass-card p-6 rounded-3xl flex gap-4 items-center">**

&#x20;                       **<div class="w-12 h-12 bg-sky-100 text-sky-600 rounded-2xl flex items-center justify-center shrink-0">**

&#x20;                           **<i data-lucide="zap" size="24"></i>**

&#x20;                       **</div>**

&#x20;                       **<div>**

&#x20;                           **<p class="font-bold text-slate-700">نتائج فورية</p>**

&#x20;                           **<p class="text-xs text-slate-400">لا حاجة للانتظار، التحليل يتم في أقل من دقيقة.</p>**

&#x20;                       **</div>**

&#x20;                   **</div>**

&#x20;               **</div>**

&#x20;           **</div>**

&#x20;       **</section>**



&#x20;       **<!-- Tracker Section -->**

&#x20;       **<section id="tracker" class="page-section">**

&#x20;           **<div class="grid grid-cols-1 lg:grid-cols-3 gap-8">**

&#x20;               **<div class="lg:col-span-2 glass-card rounded-\[2.5rem] p-8 shadow-xl border-emerald-50">**

&#x20;                   **<div class="flex justify-between items-center mb-8">**

&#x20;                       **<h3 class="text-2xl font-black flex items-center gap-2">**

&#x20;                           **<span class="w-2 h-8 bg-mix rounded-full"></span>**

&#x20;                           **سجل النشاط الصحي**

&#x20;                       **</h3>**

&#x20;                       **<div class="flex gap-2">**

&#x20;                           **<div class="flex items-center gap-1"><span class="w-3 h-3 bg-emerald-500 rounded-sm"></span> <span class="text-\[10px] text-slate-400 font-bold">ملتزم</span></div>**

&#x20;                           **<div class="flex items-center gap-1"><span class="w-3 h-3 bg-sky-400 rounded-sm"></span> <span class="text-\[10px] text-slate-400 font-bold">نشط</span></div>**

&#x20;                       **</div>**

&#x20;                   **</div>**

&#x20;                   

&#x20;                   **<div class="grid grid-cols-7 gap-3 mb-10" id="trackerGrid"></div>**

&#x20;                   

&#x20;                   **<div class="grid grid-cols-1 md:grid-cols-2 gap-6">**

&#x20;                       **<div class="p-6 bg-sky-50 rounded-2xl border border-sky-100 relative overflow-hidden group">**

&#x20;                           **<div class="absolute -bottom-4 -left-4 opacity-5 group-hover:rotate-12 transition-transform">**

&#x20;                               **<i data-lucide="droplets" size="80"></i>**

&#x20;                           **</div>**

&#x20;                           **<div class="flex justify-between items-start mb-4">**

&#x20;                               **<div class="w-12 h-12 bg-sky-500 text-white rounded-xl flex items-center justify-center">**

&#x20;                                   **<i data-lucide="droplets" size="24"></i>**

&#x20;                               **</div>**

&#x20;                               **<span class="text-xs bg-sky-200 text-sky-800 px-2 py-1 rounded-full font-bold">65% أكتمل</span>**

&#x20;                           **</div>**

&#x20;                           **<p class="text-sky-700 font-bold text-lg">النشاط المائي</p>**

&#x20;                           **<p class="text-sm text-slate-600 mt-1">شربت 5 أكواب من أصل 8 اليوم.</p>**

&#x20;                           **<div class="w-full bg-slate-200 h-2 rounded-full mt-4 overflow-hidden">**

&#x20;                               **<div class="bg-sky-500 h-full w-\[65%]"></div>**

&#x20;                           **</div>**

&#x20;                       **</div>**

&#x20;                       

&#x20;                       **<div class="p-6 bg-emerald-50 rounded-2xl border border-emerald-100 relative overflow-hidden group">**

&#x20;                           **<div class="absolute -bottom-4 -left-4 opacity-5 group-hover:rotate-12 transition-transform">**

&#x20;                               **<i data-lucide="pill" size="80"></i>**

&#x20;                           **</div>**

&#x20;                           **<div class="flex justify-between items-start mb-4">**

&#x20;                               **<div class="w-12 h-12 bg-emerald-500 text-white rounded-xl flex items-center justify-center">**

&#x20;                                   **<i data-lucide="pill" size="24"></i>**

&#x20;                               **</div>**

&#x20;                               **<span class="text-xs bg-emerald-200 text-emerald-800 px-2 py-1 rounded-full font-bold">2/3 جرعات</span>**

&#x20;                           **</div>**

&#x20;                           **<p class="text-emerald-700 font-bold text-lg">تتبع الأدوية</p>**

&#x20;                           **<p class="text-sm text-slate-600 mt-1">الموعد القادم: 9:00 مساءً</p>**

&#x20;                           **<div class="w-full bg-slate-200 h-2 rounded-full mt-4 overflow-hidden">**

&#x20;                               **<div class="bg-emerald-500 h-full w-\[66%]"></div>**

&#x20;                           **</div>**

&#x20;                       **</div>**

&#x20;                   **</div>**

&#x20;               **</div>**



&#x20;               **<!-- Step Counter (New Addition) -->**

&#x20;               **<div class="glass-card rounded-\[2.5rem] p-8 shadow-xl border-emerald-50 bg-white">**

&#x20;                   **<h3 class="text-xl font-black mb-6 flex items-center gap-2">**

&#x20;                       **<i data-lucide="footprints" class="text-emerald-500"></i> عداد الخطوات**

&#x20;                   **</h3>**

&#x20;                   **<div class="flex flex-col items-center py-10">**

&#x20;                       **<div class="relative w-40 h-40 flex items-center justify-center">**

&#x20;                            **<svg class="w-full h-full transform -rotate-90">**

&#x20;                               **<circle cx="80" cy="80" r="70" stroke="currentColor" stroke-width="12" fill="transparent" class="text-slate-100" />**

&#x20;                               **<circle cx="80" cy="80" r="70" stroke="currentColor" stroke-width="12" fill="transparent" stroke-dasharray="440" stroke-dashoffset="110" class="text-emerald-500" />**

&#x20;                           **</svg>**

&#x20;                           **<div class="absolute flex flex-col items-center">**

&#x20;                               **<span class="text-3xl font-black text-slate-800">7,240</span>**

&#x20;                               **<span class="text-\[10px] text-slate-400 font-bold">خطوة اليوم</span>**

&#x20;                           **</div>**

&#x20;                       **</div>**

&#x20;                       **<p class="mt-6 text-sm text-slate-500 font-medium">هدفك: 10,000 خطوة</p>**

&#x20;                   **</div>**

&#x20;                   **<div class="space-y-4">**

&#x20;                       **<div class="flex justify-between items-center text-xs">**

&#x20;                           **<span class="text-slate-400 font-bold uppercase">السعرات المحروقة</span>**

&#x20;                           **<span class="text-slate-700 font-black">320 سعرة</span>**

&#x20;                       **</div>**

&#x20;                       **<div class="w-full h-1 bg-slate-100 rounded-full"></div>**

&#x20;                       **<div class="flex justify-between items-center text-xs">**

&#x20;                           **<span class="text-slate-400 font-bold uppercase">المسافة</span>**

&#x20;                           **<span class="text-slate-700 font-black">5.4 كم</span>**

&#x20;                       **</div>**

&#x20;                       **<div class="w-full h-1 bg-slate-100 rounded-full"></div>**

&#x20;                   **</div>**

&#x20;               **</div>**

&#x20;           **</div>**

&#x20;       **</section>**



&#x20;       **<!-- Emergency Section -->**

&#x20;       **<section id="emergency" class="page-section">**

&#x20;           **<div class="max-w-md mx-auto glass-card rounded-\[2.5rem] p-10 text-center shadow-2xl border-2 border-red-50">**

&#x20;               **<div class="w-20 h-20 bg-red-50 text-red-600 rounded-full flex items-center justify-center mx-auto mb-6 pulse-anim">**

&#x20;                   **<i data-lucide="alert-triangle" size="40"></i>**

&#x20;               **</div>**

&#x20;               **<h2 class="text-3xl font-black text-red-600 mb-4">خدمة الاستغاثة</h2>**

&#x20;               **<p class="text-slate-500 mb-8 leading-relaxed">بمجرد الضغط، سيتم إرسال موقعك الجغرافي الدقيق وملفك الطبي لأقرب وحدة طوارئ.</p>**

&#x20;               **<button class="w-full bg-red-600 text-white py-5 rounded-2xl text-xl font-bold shadow-xl shadow-red-200 hover:bg-red-700 transition active:scale-95">اتصل الآن 997</button>**

&#x20;               **<p class="text-\[10px] text-slate-400 mt-6 italic">\* تعمل هذه الخدمة بالتنسيق مع الهلال الأحمر السعودي</p>**

&#x20;           **</div>**

&#x20;       **</section>**



&#x20;   **</main>**



&#x20;   **<!-- Footer -->**

&#x20;   **<footer class="bg-white border-t border-emerald-50 py-16 mt-20">**

&#x20;       **<div class="container mx-auto px-4">**

&#x20;           **<div class="flex flex-col md:flex-row justify-between items-center gap-10 mb-12">**

&#x20;               **<div class="flex flex-col items-center md:items-start text-center md:text-right gap-3">**

&#x20;                   **<div class="flex items-center gap-3">**

&#x20;                       **<div class="w-10 h-10 bg-mix rounded-lg shadow-sm flex items-center justify-center p-2">**

&#x20;                           **<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-white">**

&#x20;                               **<path d="M3 12H7L9 5L12 19L15 9L17 12H21" stroke="currentColor" stroke-width="3" stroke-linecap="round" stroke-linejoin="round"/>**

&#x20;                           **</svg>**

&#x20;                       **</div>**

&#x20;                       **<span class="font-black text-2xl text-gradient">خُـطـى</span>**

&#x20;                   **</div>**

&#x20;                   **<p class="text-slate-400 text-sm max-w-xs mt-2">نبتكر الحلول الصحية لنرسم غداً أفضل، مدعومين بقوة الذكاء الاصطناعي.</p>**

&#x20;               **</div>**

&#x20;               

&#x20;               **<div class="flex flex-wrap justify-center gap-8">**

&#x20;                   **<div class="flex flex-col items-center md:items-start">**

&#x20;                       **<h4 class="font-black text-slate-800 mb-4 text-sm">عن خُطى</h4>**

&#x20;                       **<ul class="text-xs text-slate-500 space-y-2 font-bold">**

&#x20;                           **<li class="hover:text-medical-600 cursor-pointer">الرؤية والرسالة</li>**

&#x20;                           **<li class="hover:text-medical-600 cursor-pointer">فريق العمل</li>**

&#x20;                           **<li class="hover:text-medical-600 cursor-pointer">الابتكار</li>**

&#x20;                       **</ul>**

&#x20;                   **</div>**

&#x20;                   **<div class="flex flex-col items-center md:items-start">**

&#x20;                       **<h4 class="font-black text-slate-800 mb-4 text-sm">الدعم</h4>**

&#x20;                       **<ul class="text-xs text-slate-500 space-y-2 font-bold">**

&#x20;                           **<li class="hover:text-medical-600 cursor-pointer">الأسئلة الشائعة</li>**

&#x20;                           **<li class="hover:text-medical-600 cursor-pointer">سياسة الخصوصية</li>**

&#x20;                           **<li class="hover:text-medical-600 cursor-pointer">تواصل معنا</li>**

&#x20;                       **</ul>**

&#x20;                   **</div>**

&#x20;               **</div>**

&#x20;           **</div>**

&#x20;           

&#x20;           **<div class="text-center pt-8 border-t border-slate-50">**

&#x20;               **<p class="text-slate-500 font-medium">إشراف الطالبة: <span class="text-slate-800 font-bold">دانة بدر حمد المطيري</span></p>**

&#x20;               **<div class="flex justify-center gap-6 mt-6 text-slate-300">**

&#x20;                   **<i data-lucide="instagram" size="20" class="hover:text-pink-500 transition cursor-pointer"></i>**

&#x20;                   **<i data-lucide="twitter" size="20" class="hover:text-sky-500 transition cursor-pointer"></i>**

&#x20;                   **<i data-lucide="linkedin" size="20" class="hover:text-blue-700 transition cursor-pointer"></i>**

&#x20;               **</div>**

&#x20;               **<p class="text-\[10px] text-slate-300 mt-10 uppercase tracking-\[0.2em]">© 2026 KHUTA HEALTHCARE SOLUTIONS - INNOVATIVE MEDICAL SOLUTIONS</p>**

&#x20;           **</div>**

&#x20;       **</div>**

&#x20;   **</footer>**



&#x20;   **<script>**

&#x20;       **lucide.createIcons();**



&#x20;       **// Tracker Grid Generation (Enhanced)**

&#x20;       **const grid = document.getElementById('trackerGrid');**

&#x20;       **for(let i=1; i<=28; i++) {**

&#x20;           **let bgColor = i < 18 ? 'bg-emerald-500' : (i < 24 ? 'bg-sky-400' : 'bg-slate-100');**

&#x20;           **let opacity = Math.random() \* (1 - 0.5) + 0.5;**

&#x20;           **grid.innerHTML += `<div class="h-10 rounded-lg ${bgColor} shadow-sm transition-all hover:scale-110 cursor-pointer hover:shadow-lg" style="opacity: ${opacity}" title="اليوم ${i}"></div>`;**

&#x20;       **}**



&#x20;       **function showPage(id) {**

&#x20;           **document.querySelectorAll('.page-section').forEach(s => s.classList.remove('active'));**

&#x20;           **document.getElementById(id).classList.add('active');**

&#x20;           

&#x20;           **document.querySelectorAll('.nav-btn').forEach(btn => {**

&#x20;               **btn.classList.remove('active-link');**

&#x20;               **if(btn.innerText.includes(getButtonText(id))) btn.classList.add('active-link');**

&#x20;           **});**

&#x20;           **window.scrollTo({ top: 0, behavior: 'smooth' });**

&#x20;       **}**



&#x20;       **function getButtonText(id) {**

&#x20;           **const map = {'home':'الرئيسية', 'bot':'المساعد', 'analysis':'تحليل', 'tracker':'تتبع', 'emergency':'طوارئ'};**

&#x20;           **return map\[id] || '';**

&#x20;       **}**



&#x20;       **function quickAsk(text) {**

&#x20;           **document.getElementById('chatInput').value = text;**

&#x20;           **sendMessage();**

&#x20;       **}**



&#x20;       **function sendMessage() {**

&#x20;           **const input = document.getElementById('chatInput');**

&#x20;           **const history = document.getElementById('chatHistory');**

&#x20;           **if(!input.value.trim()) return;**



&#x20;           **const userText = input.value;**

&#x20;           **history.innerHTML += `**

&#x20;               **<div class="flex justify-end gap-3 animate-in slide-in-from-left-2 duration-300">**

&#x20;                   **<div class="bg-mix text-white p-4 rounded-2xl rounded-tl-none shadow-sm text-sm max-w-\[85%] font-medium">**

&#x20;                       **${userText}**

&#x20;                   **</div>**

&#x20;               **</div>**

&#x20;           **`;**

&#x20;           **input.value = '';**

&#x20;           **history.scrollTop = history.scrollHeight;**

&#x20;           

&#x20;           **setTimeout(() => {**

&#x20;               **let response = "نظام خُطى الذكي يقوم بمعالجة استفسارك الآن... هل تود معرفة المزيد عن هذا الموضوع؟";**

&#x20;               

&#x20;               **// Enhanced Bot Logic**

&#x20;               **if(userText.includes("ألم") || userText.includes("صداع")) {**

&#x20;                   **response = "يؤسفني شعورك بالألم. هل هذا الصداع مفاجئ؟ وهل يصاحبه غثيان أو زغللة في العين؟ (تذكر أن تشخيصي استرشادي)";**

&#x20;               **} else if (userText.includes("موعد") || userText.includes("حجز")) {**

&#x20;                   **response = "بالتأكيد، يمكنني البدء بإجراءات الحجز. هل تود البحث عن أقرب مستشفى متاح أم عيادة تخصصية معينة؟";**

&#x20;               **} else if (userText.includes("غذاء") || userText.includes("نصيحة")) {**

&#x20;                   **response = "بناءً على ملفك، ننصحك بزيادة الألياف وشرب المزيد من الماء. هل ترغب في وضع جدول غذائي مخصص؟";**

&#x20;               **}**

&#x20;               

&#x20;               **history.innerHTML += `**

&#x20;                   **<div class="flex gap-3 text-right animate-in slide-in-from-right-2 duration-300">**

&#x20;                       **<div class="w-8 h-8 bg-sky-100 text-sky-600 rounded-full flex items-center justify-center flex-shrink-0">**

&#x20;                           **<i data-lucide="bot" size="18"></i>**

&#x20;                       **</div>**

&#x20;                       **<div class="bg-white p-4 rounded-2xl rounded-tr-none shadow-sm border border-emerald-50 max-w-\[85%] text-sm leading-relaxed">**

&#x20;                           **${response}**

&#x20;                       **</div>**

&#x20;                   **</div>**

&#x20;               **`;**

&#x20;               **lucide.createIcons();**

&#x20;               **history.scrollTop = history.scrollHeight;**

&#x20;           **}, 1000);**

&#x20;       **}**



&#x20;       **function handleFile(input) {**

&#x20;           **if(!input.files\[0]) return;**

&#x20;           **const res = document.getElementById('fileResult');**

&#x20;           

&#x20;           **res.innerHTML = `**

&#x20;               **<div class="flex flex-col items-center py-6">**

&#x20;                   **<div class="w-12 h-12 border-4 border-emerald-500 border-t-transparent rounded-full animate-spin mb-4"></div>**

&#x20;                   **<p class="text-emerald-600 font-black">جاري تحليل بيانات التقرير باستخدام محرك خُطى...</p>**

&#x20;               **</div>**

&#x20;           **`;**

&#x20;           **res.classList.remove('hidden');**



&#x20;           **setTimeout(() => {**

&#x20;               **res.innerHTML = `**

&#x20;                   **<h4 class="font-black text-medical-700 mb-4 flex items-center gap-2">**

&#x20;                       **<i data-lucide="check-circle" size="20"></i> ملخص التحليل الذكي:**

&#x20;                   **</h4>**

&#x20;                   **<div class="space-y-4">**

&#x20;                       **<div class="p-3 bg-red-50 rounded-xl border border-red-100 flex justify-between items-center">**

&#x20;                           **<div>**

&#x20;                               **<p class="text-xs font-bold text-red-700">مستوى الهيموجلوبين</p>**

&#x20;                               **<p class="text-\[10px] text-red-500 font-medium">يوجد انخفاض بسيط عن المعدل الطبيعي</p>**

&#x20;                           **</div>**

&#x20;                           **<span class="text-lg font-black text-red-600">10.5</span>**

&#x20;                       **</div>**

&#x20;                       **<div class="p-3 bg-emerald-50 rounded-xl border border-emerald-100 flex justify-between items-center">**

&#x20;                           **<div>**

&#x20;                               **<p class="text-xs font-bold text-emerald-700">مستوى السكر (صائم)</p>**

&#x20;                               **<p class="text-\[10px] text-emerald-500 font-medium">ضمن الحدود الطبيعية</p>**

&#x20;                           **</div>**

&#x20;                           **<span class="text-lg font-black text-emerald-600">88</span>**

&#x20;                       **</div>**

&#x20;                   **</div>**

&#x20;                   **<div class="mt-6 p-4 bg-sky-50 rounded-2xl text-xs text-sky-800 leading-relaxed font-bold border border-sky-100">**

&#x20;                       **<i data-lucide="lightbulb" size="14" class="inline mb-1 ml-1"></i>**

&#x20;                       **تفسير خُطى: تظهر النتائج بوادر فقر دم (أنيميا). يُنصح بتناول الأغذية الغنية بالحديد ومراجعة الطبيب.**

&#x20;                   **</div>**

&#x20;               **`;**

&#x20;               **lucide.createIcons();**

&#x20;           **}, 2500);**

&#x20;       **}**



&#x20;       **document.getElementById('chatInput').addEventListener('keypress', (e) => {**

&#x20;           **if(e.key === 'Enter') sendMessage();**

&#x20;       **});**

&#x20;   **</script>**



&#x20;   **<style>**

&#x20;       **.pulse-anim {**

&#x20;           **animation: pulse-ring 2s infinite;**

&#x20;       **}**

&#x20;       **@keyframes pulse-ring {**

&#x20;           **0% { box-shadow: 0 0 0 0 rgba(220, 38, 38, 0.4); }**

&#x20;           **70% { box-shadow: 0 0 0 15px rgba(220, 38, 38, 0); }**

&#x20;           **100% { box-shadow: 0 0 0 0 rgba(220, 38, 38, 0); }**

&#x20;       **}**

&#x20;   **</style>**

**</body>**

**</html>**


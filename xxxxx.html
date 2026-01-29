<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">
    <title>Zihad Brand - Box Layout Pro</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root { --sat: env(safe-area-inset-top); --sab: env(safe-area-inset-bottom); }
        * { box-sizing: border-box; -webkit-tap-highlight-color: transparent; margin: 0; padding: 0; }
        
        body, html { 
            height: 100%; width: 100%; 
            background: #000; overflow: hidden; 
            position: fixed; display: flex; align-items: center; justify-content: center;
        }

        /* গোপন ট্রিগার (কোণায় ডাবল ক্লিক) */
        #admin-trigger-right { position: fixed; top: 0; right: 0; width: 45px; height: 45px; z-index: 10000; }
        #admin-trigger-left { position: fixed; top: 0; left: 0; width: 45px; height: 45px; z-index: 10000; }

        /* মেইন কন্টেইনার - বক্স লেআউট */
        .app-box {
            width: 95vw; height: 96vh; /* বক্সের শেপ দেওয়ার জন্য কিছুটা কমানো হয়েছে */
            background: radial-gradient(circle at center, #050510, #000);
            display: flex; flex-direction: column;
            position: relative; overflow: hidden;
            border: 3px solid;
            border-radius: 20px; /* বক্সের চারকোনা গোল */
            animation: boxGlow 3s linear infinite;
        }

        @keyframes boxGlow {
            0%, 100% { border-color: #ff0000; box-shadow: 0 0 30px rgba(255, 0, 0, 0.4), inset 0 0 20px rgba(255, 0, 0, 0.2); }
            50% { border-color: #0000ff; box-shadow: 0 0 30px rgba(0, 0, 255, 0.4), inset 0 0 20px rgba(0, 0, 255, 0.2); }
        }

        /* কন্টেন্ট স্ক্রল */
        .content-scroll { 
            flex: 1; overflow-y: auto; 
            padding: 20px; padding-bottom: 150px; /* সোশ্যাল বারের জন্য গ্যাপ */
            scrollbar-width: none; 
        }
        .content-scroll::-webkit-scrollbar { display: none; }

        /* ঝিলমিল কার্ড ও প্রোফাইল */
        .jhilmil { 
            animation: jhilmilAnim 2s linear infinite; 
            border: 2px solid; 
        }
        @keyframes jhilmilAnim {
            0% { border-color: #ff0055; box-shadow: 0 0 10px #ff0055; }
            50% { border-color: #0088ff; box-shadow: 0 0 10px #0088ff; }
            100% { border-color: #ff0055; box-shadow: 0 0 10px #ff0055; }
        }

        /* সোশ্যাল মিডিয়া বার - একটু উপরে উঠানো */
        .floating-social {
            position: absolute; 
            bottom: 60px; /* নিচ থেকে উপরে উঠানো হয়েছে */
            left: 50%; transform: translateX(-50%);
            width: 80%; max-width: 260px; 
            background: rgba(10, 10, 25, 0.8);
            backdrop-filter: blur(20px); 
            border: 1.5px solid rgba(255, 255, 255, 0.1);
            border-radius: 40px; 
            display: flex; justify-content: space-around;
            padding: 10px; z-index: 5000;
            box-shadow: 0 15px 35px rgba(0,0,0,0.8);
        }

        /* সোশ্যাল বাটন হাইলাইট এনিমেশন */
        .nav-item {
            position: relative; width: 45px; height: 45px;
            display: flex; align-items: center; justify-content: center;
            border-radius: 50%; font-size: 20px; color: #fff;
            transition: 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }
        .nav-item:active {
            background: rgba(255, 255, 255, 0.15);
            transform: scale(1.4) translateY(-15px);
            box-shadow: 0 0 25px currentColor;
        }

        /* Modals */
        .modal { position: fixed; inset: 0; background: rgba(0,0,0,0.95); display: none; overflow-y: auto; z-index: 20000; padding: 20px; align-items: center; justify-content: center; }
        .admin-box { background: #080810; border: 2px solid #3b82f6; padding: 25px; width: 100%; max-width: 350px; border-radius: 15px; }
        input, textarea { width: 100%; background: #111; border: 1px solid #222; color: #fff; padding: 12px; margin-bottom: 10px; font-size: 13px; outline: none; border-radius: 5px; }
    </style>
</head>
<body onload="loadData()">

    <div id="admin-trigger-right" ondblclick="openModal('admin-modal')"></div>
    <div id="admin-trigger-left" ondblclick="openModal('delete-modal')"></div>

    <div class="app-box">
        <div class="content-scroll">
            <div class="flex flex-col items-center text-center mt-8 mb-8">
                <div class="w-24 h-24 overflow-hidden bg-black mb-4 jhilmil rounded-full">
                    <img src="https://via.placeholder.com/150" id="display-logo" class="w-full h-full object-cover">
                </div>
                <h1 id="display-name" class="text-2xl font-black text-white uppercase tracking-tighter italic">ZIHAD BRAND</h1>
                <div class="h-1 w-16 bg-blue-600 mx-auto mt-2 animate-pulse"></div>
            </div>

            <div class="square-card jhilmil p-4 rounded-xl mb-8">
                <p id="display-bio" class="text-gray-300 text-xs text-center leading-relaxed">আপনার বায়ো এখানে থাকবে।</p>
            </div>

            <div id="project-container"></div>
        </div>

        <div class="floating-social jhilmil">
            <a id="fb-link" href="#" target="_blank" class="nav-item text-blue-500"><i class="fa-brands fa-facebook-f"></i></a>
            <a id="wa-link" href="#" target="_blank" class="nav-item text-green-500"><i class="fa-brands fa-whatsapp"></i></a>
            <a id="tg-link" href="#" target="_blank" class="nav-item text-sky-400"><i class="fa-brands fa-telegram-plane"></i></a>
            <a href="#" class="nav-item text-pink-500"><i class="fa-brands fa-instagram"></i></a>
        </div>
    </div>

    <div id="admin-modal" class="modal">
        <div class="admin-box">
            <h2 class="text-white font-bold mb-4 text-center uppercase border-b border-blue-900 pb-2">Admin Control</h2>
            <input type="text" id="logo-input" placeholder="Logo URL">
            <input type="text" id="name-input" placeholder="Name">
            <textarea id="bio-input" placeholder="Bio..."></textarea>
            <input type="text" id="fb-in" placeholder="FB Link">
            <input type="text" id="wa-in" placeholder="WA Number">
            <input type="text" id="tg-in" placeholder="Telegram Link">
            <hr class="my-4 border-gray-800">
            <input type="text" id="p-img" placeholder="Project Image Link">
            <input type="text" id="p-title" placeholder="Project Title">
            <input type="text" id="p-video" placeholder="Direct Link (3rd Click)">
            <button onclick="saveAll()" class="w-full bg-blue-700 py-3 font-bold text-white mt-2 rounded">SAVE ALL</button>
            <button onclick="closeModals()" class="w-full bg-gray-900 py-2 mt-2 text-xs text-white">CLOSE</button>
        </div>
    </div>

    <div id="delete-modal" class="modal">
        <div class="admin-box">
            <h2 class="text-red-500 font-bold mb-4 text-center border-b border-red-900 pb-2">DELETE PANEL</h2>
            <div id="delete-list" class="max-h-60 overflow-y-auto mb-4"></div>
            <button onclick="closeModals()" class="w-full bg-red-900 py-3 font-bold text-white">CLOSE</button>
        </div>
    </div>

    <script>
        let clickCount = 0;
        const adLink = "https://www.effectivegatecpm.com/wzacd8ppk?key=d5926c0ef7c1dc7212610c458cd5ff37";

        function openModal(id) { document.getElementById(id).style.display = 'flex'; if(id === 'delete-modal') renderDeleteList(); }
        function closeModals() { document.querySelectorAll('.modal').forEach(m => m.style.display = 'none'); }

        function handleProjectClick(finalUrl) {
            clickCount++;
            if (clickCount < 3) { window.open(adLink, '_blank'); } 
            else { window.open(finalUrl, '_blank'); clickCount = 0; }
        }

        function saveAll() {
            const current = JSON.parse(localStorage.getItem('z_data')) || { profile: {}, projects: [] };
            const profile = {
                logo: document.getElementById('logo-input').value || current.profile.logo || "https://via.placeholder.com/150",
                name: document.getElementById('name-input').value || current.profile.name || "ZIHAD BRAND",
                bio: document.getElementById('bio-input').value || current.profile.bio || "আপনার বায়ো এখানে থাকবে।",
                fb: document.getElementById('fb-in').value || current.profile.fb || "#",
                wa: document.getElementById('wa-in').value || current.profile.wa || "",
                tg: document.getElementById('tg-in').value || current.profile.tg || "#"
            };
            if(document.getElementById('p-img').value && document.getElementById('p-title').value) {
                current.projects.push({ img: document.getElementById('p-img').value, title: document.getElementById('p-title').value, video: document.getElementById('p-video').value });
            }
            localStorage.setItem('z_data', JSON.stringify({ profile, projects: current.projects }));
            location.reload(); 
        }

        function loadData() {
            const data = JSON.parse(localStorage.getItem('z_data'));
            if(!data) return;
            document.getElementById('display-logo').src = data.profile.logo;
            document.getElementById('display-name').innerText = data.profile.name;
            document.getElementById('display-bio').innerText = data.profile.bio;
            document.getElementById('fb-link').href = data.profile.fb;
            document.getElementById('wa-link').href = data.profile.wa ? "https://wa.me/" + data.profile.wa : "#";
            document.getElementById('tg-link').href = data.profile.tg;

            const container = document.getElementById('project-container');
            container.innerHTML = "";
            data.projects.forEach((p) => {
                container.innerHTML += `
                <div class="square-card !p-0 overflow-hidden jhilmil rounded-2xl mb-6" onclick="handleProjectClick('${p.video || '#'}')">
                    <img src="${p.img}" class="w-full h-44 object-cover">
                    <div class="p-3 bg-black/95 flex justify-between items-center">
                        <h4 class="text-blue-400 font-bold text-[10px] uppercase">${p.title}</h4>
                        <i class="fa-solid fa-play text-red-600 animate-pulse"></i>
                    </div>
                </div>`;
            });
        }

        function renderDeleteList() {
            const data = JSON.parse(localStorage.getItem('z_data')) || { projects: [] };
            const list = document.getElementById('delete-list');
            list.innerHTML = "";
            data.projects.forEach((p, index) => {
                list.innerHTML += `<div class="flex justify-between items-center bg-gray-900 p-3 rounded mb-2"><span class="text-white text-xs">${p.title}</span><button onclick="deleteProject(${index})" class="bg-red-600 text-[10px] px-3 py-1 rounded">DEL</button></div>`;
            });
        }

        function deleteProject(index) {
            let data = JSON.parse(localStorage.getItem('z_data'));
            data.projects.splice(index, 1);
            localStorage.setItem('z_data', JSON.stringify(data));
            renderDeleteList(); loadData();
        }
    </script>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chaat Puchka - Franchise Login</title>
    <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-orange-700 flex justify-center items-center min-h-screen m-0 p-4 relative overflow-hidden">
    <!-- Glowing atmosphere circles -->
    <div class="absolute top-1/4 left-1/4 w-80 h-80 rounded-full bg-amber-500 opacity-20 blur-3xl pointer-events-none"></div>
    <div class="absolute bottom-1/4 right-1/4 w-80 h-80 rounded-full bg-orange-600 opacity-20 blur-3xl pointer-events-none"></div>

    <div class="bg-black/30 backdrop-blur-xl p-6 sm:p-8 rounded-3xl shadow-2xl w-full max-w-sm text-center border border-white/20 relative z-10 text-white">
        <div class="mb-6 flex flex-col items-center">
            <div class="w-24 h-24 sm:w-28 sm:h-28 bg-black/60 rounded-2xl flex items-center justify-center p-2 mb-3 shadow-xl border border-white/10">
                <img src="https://i.postimg.cc/SsSZBQ9q/1000037254-removebg-preview.png" alt="Chaat Puchka Logo" class="w-full h-full object-contain">
            </div>
            <h2 class="text-2xl font-black tracking-tight text-white drop-shadow">Franchise Portal</h2>
            <p class="text-xs text-emerald-300 font-bold mt-1 tracking-wide">Manage your outlet & live orders</p>
        </div>
        
        <input type="text" id="loginId" placeholder="Login ID" class="w-full p-3.5 mb-3 bg-white/15 backdrop-blur-md border border-white/30 placeholder-white/60 text-white rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-emerald-400 box-border font-bold">
        <input type="password" id="password" placeholder="Password" class="w-full p-3.5 mb-4 bg-white/15 backdrop-blur-md border border-white/30 placeholder-white/60 text-white rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-emerald-400 box-border font-bold">
        
        <button onclick="franchiseLogin()" class="w-full bg-emerald-500 hover:bg-emerald-600 text-white font-black p-3.5 rounded-xl shadow-lg transition transform active:scale-95">Login to Dashboard ⚡</button>
        <div id="error-msg" class="text-red-300 text-xs mt-3 font-semibold"></div>
    </div>

    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/10.8.0/firebase-app.js";
        import { getDatabase, ref, get, child } from "https://www.gstatic.com/firebasejs/10.8.0/firebase-database.js";

        const firebaseConfig = {
            databaseURL: "https://teat-2-4b868-default-rtdb.europe-west1.firebasedatabase.app/"
        };
        const app = initializeApp(firebaseConfig);
        const db = getDatabase(app);

        window.franchiseLogin = function() {
            const inputId = document.getElementById('loginId').value.trim();
            const inputPass = document.getElementById('password').value.trim();
            const errorDiv = document.getElementById('error-msg');
            errorDiv.textContent = '';

            if (!inputId || !inputPass) {
                errorDiv.textContent = 'Please fill out all fields.';
                return;
            }

            get(child(ref(db), 'franchises')).then((snapshot) => {
                if (snapshot.exists()) {
                    let found = false;
                    snapshot.forEach((childSnap) => {
                        let branch = childSnap.val();
                        if (branch.loginId === inputId && branch.password === inputPass) {
                            found = true;
                            window.location.href = `franchise.html?branchId=${childSnap.key}&branchName=${encodeURIComponent(branch.name)}`;
                        }
                    });
                    if (!found) {
                        errorDiv.textContent = 'Invalid Login ID or Password.';
                    }
                }
            });
        };
    </script>
</body>
</html>

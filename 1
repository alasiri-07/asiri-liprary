<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>قائمتي - متتبع الوسائط الشخصي</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;500;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Tajawal', sans-serif;
            scroll-behavior: smooth;
        }
        .modal-backdrop {
            display: none; position: fixed; top: 0; left: 0; right: 0; bottom: 0;
            background-color: rgba(0, 0, 0, 0.7); z-index: 40; animation: fadeIn 0.3s ease-out;
        }
        .modal {
            display: none; position: fixed; top: 50%; left: 50%;
            transform: translate(-50%, -50%); z-index: 50; animation: slideInUp 0.4s ease-out;
        }
        .modal.show, .modal-backdrop.show { display: block; }
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }
        @keyframes slideInUp { from { transform: translate(-50%, -40%); opacity: 0; } to { transform: translate(-50%, -50%); opacity: 1; } }
        
        .star-rating input[type="radio"] { display: none; }
        .star-rating label { font-size: 2rem; color: #4a5568; cursor: pointer; transition: color 0.2s; }
        .star-rating input[type="radio"]:checked ~ label,
        .star-rating:hover label,
        .star-rating label:hover ~ label { color: #f59e0b; }
        .star-rating input[type="radio"]:hover ~ label { color: #f59e0b; }

        .media-card {
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }
        .media-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 10px 25px -5px rgba(13, 187, 215, 0.2), 0 8px 10px -6px rgba(13, 187, 215, 0.2);
        }
        
        #snackbar {
            visibility: hidden; min-width: 250px; margin-left: -125px; background-color: #ef4444;
            color: #fff; text-align: center; border-radius: 8px; padding: 16px; position: fixed;
            z-index: 100; left: 50%; bottom: 30px; font-size: 17px;
            transition: visibility 0s, opacity 0.5s linear; opacity: 0;
        }
        #snackbar.show { visibility: visible; opacity: 1; }
        
        .status-badge {
            position: absolute; top: 12px; left: 12px; padding: 4px 10px;
            border-radius: 9999px; font-size: 12px; font-weight: bold;
            text-transform: uppercase; letter-spacing: 0.5px;
        }
    </style>
</head>
<body class="bg-gray-900 text-white">

    <!-- Header -->
    <header class="bg-gray-800/80 backdrop-blur-sm shadow-lg p-4 sticky top-0 z-30 border-b border-gray-700">
        <div class="container mx-auto flex justify-between items-center">
            <h1 class="text-2xl font-bold text-cyan-400">قائمتي</h1>
            <button id="addItemBtn" class="bg-cyan-500 hover:bg-cyan-600 text-white font-bold py-2 px-4 rounded-lg flex items-center gap-2 transition-transform transform hover:scale-105">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M10 3a1 1 0 011 1v5h5a1 1 0 110 2h-5v5a1 1 0 11-2 0v-5H4a1 1 0 110-2h5V4a1 1 0 011-1z" clip-rule="evenodd" /></svg>
                <span>إضافة عمل جديد</span>
            </button>
        </div>
    </header>

    <!-- Categories Navigation -->
    <nav class="bg-gray-800 border-b border-gray-700">
        <div class="container mx-auto">
            <div id="category-tabs" class="flex items-center justify-center sm:justify-start overflow-x-auto whitespace-nowrap p-2"></div>
        </div>
    </nav>

    <!-- Main Content -->
    <main class="container mx-auto p-4 md:p-6">
        <div class="flex flex-col md:flex-row justify-between items-center mb-6 gap-4">
            <h2 id="category-title" class="text-3xl font-bold text-cyan-300"></h2>
            <div class="relative w-full md:w-1/3">
                <input type="text" id="searchInput" placeholder="ابحث في هذا القسم..." class="w-full bg-gray-700 border border-gray-600 rounded-lg px-4 py-2 pr-10 focus:ring-cyan-500 focus:border-cyan-500 transition">
                <svg class="w-5 h-5 text-gray-400 absolute top-1/2 right-3 transform -translate-y-1/2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z" clip-rule="evenodd" /></svg>
            </div>
        </div>
        <div id="items-grid" class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5 gap-6"></div>
        <div id="empty-state" class="hidden text-center py-16">
            <svg xmlns="http://www.w3.org/2000/svg" class="mx-auto h-20 w-20 text-gray-600" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1"><path stroke-linecap="round" stroke-linejoin="round" d="M5 8h14M5 8a2 2 0 110-4h14a2 2 0 110 4M5 8v10a2 2 0 002 2h10a2 2 0 002-2V8m-9 4h4" /></svg>
            <h3 class="mt-4 text-xl font-medium text-gray-300">هذا القسم فارغ حالياً</h3>
            <p class="mt-1 text-gray-400">هل أنت مستعد لاكتشاف شيء جديد؟ أضف أول عمل لك!</p>
        </div>
    </main>

    <!-- Add/Edit Item Modal -->
    <div id="itemModalBackdrop" class="modal-backdrop"></div>
    <div id="itemModal" class="modal w-11/12 md:w-2/3 lg:w-1/2 max-w-4xl bg-gray-800 rounded-2xl shadow-2xl border border-gray-700">
        <div class="p-6 md:p-8">
            <form id="itemForm" class="space-y-6">
                <div class="flex justify-between items-center mb-6">
                    <h3 id="modal-title" class="text-2xl font-bold text-cyan-400">إضافة عمل جديد</h3>
                    <button type="button" id="closeModalBtn" class="text-gray-400 hover:text-white"><svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" /></svg></button>
                </div>
                <input type="hidden" id="itemId">
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                    <div><label for="itemName" class="block text-sm font-medium text-gray-300 mb-2">اسم العمل</label><input type="text" id="itemName" class="w-full bg-gray-700 border border-gray-600 rounded-lg px-3 py-2 focus:ring-cyan-500 focus:border-cyan-500 transition" required></div>
                    <div><label for="itemCategory" class="block text-sm font-medium text-gray-300 mb-2">القسم</label><select id="itemCategory" class="w-full bg-gray-700 border border-gray-600 rounded-lg px-3 py-2 focus:ring-cyan-500 focus:border-cyan-500 transition" required></select></div>
                </div>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                    <div><label for="itemStatus" class="block text-sm font-medium text-gray-300 mb-2">الحالة</label><select id="itemStatus" class="w-full bg-gray-700 border border-gray-600 rounded-lg px-3 py-2 focus:ring-cyan-500 focus:border-cyan-500 transition"></select></div>
                    <div><label for="itemProgress" class="block text-sm font-medium text-gray-300 mb-2">آخر فصل/حلقة</label><input type="text" id="itemProgress" class="w-full bg-gray-700 border border-gray-600 rounded-lg px-3 py-2 focus:ring-cyan-500 focus:border-cyan-500 transition" placeholder="مثال: الفصل 120"></div>
                </div>
                <div><label for="itemImageUrl" class="block text-sm font-medium text-gray-300 mb-2">رابط الصورة (اختياري)</label><input type="url" id="itemImageUrl" class="w-full bg-gray-700 border border-gray-600 rounded-lg px-3 py-2 focus:ring-cyan-500 focus:border-cyan-500 transition" placeholder="https://example.com/image.jpg"></div>
                <div><label for="itemStory" class="block text-sm font-medium text-gray-300 mb-2">القصة/الوصف</label><textarea id="itemStory" rows="3" class="w-full bg-gray-700 border border-gray-600 rounded-lg px-3 py-2 focus:ring-cyan-500 focus:border-cyan-500 transition"></textarea></div>
                <div><label class="block text-sm font-medium text-gray-300 mb-2">تقييمك الشخصي</label><div id="itemRating" class="star-rating flex flex-row-reverse justify-end items-center"></div></div>
                <div class="border-t border-gray-700 pt-6">
                    <div class="flex justify-between items-center mb-4"><h4 class="text-lg font-semibold text-gray-200">فصول/لحظات مهمة</h4><button type="button" id="addMomentBtn" class="bg-gray-600 hover:bg-gray-500 text-white font-bold py-2 px-3 rounded-lg flex items-center gap-2 text-sm"><svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M10 3a1 1 0 011 1v5h5a1 1 0 110 2h-5v5a1 1 0 11-2 0v-5H4a1 1 0 110-2h5V4a1 1 0 011-1z" clip-rule="evenodd" /></svg>إضافة</button></div>
                    <div id="moments-container" class="space-y-4 max-h-48 overflow-y-auto pr-2"></div>
                </div>
                <div class="flex justify-end gap-4 pt-4">
                    <button type="button" id="deleteItemBtn" class="hidden bg-red-600 hover:bg-red-700 text-white font-bold py-2 px-6 rounded-lg transition">حذف</button>
                    <button type="submit" class="bg-cyan-500 hover:bg-cyan-600 text-white font-bold py-2 px-8 rounded-lg transition">حفظ</button>
                </div>
            </form>
        </div>
    </div>
    
    <!-- View Item Modal -->
    <div id="viewModalBackdrop" class="modal-backdrop"></div>
    <div id="viewModal" class="modal w-11/12 md:w-2/3 lg:w-1/2 max-w-4xl bg-gray-800 rounded-2xl shadow-2xl border border-gray-700">
         <div class="p-6 md:p-8 relative"><button id="closeViewModalBtn" class="absolute top-4 left-4 text-gray-400 hover:text-white z-10"><svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" /></svg></button><div id="view-content" class="space-y-6"></div><div class="mt-8 flex justify-end"><button id="editItemBtn" class="bg-cyan-500 hover:bg-cyan-600 text-white font-bold py-2 px-6 rounded-lg transition">تعديل</button></div></div>
    </div>

    <!-- Confirmation Modal -->
    <div id="confirmModalBackdrop" class="modal-backdrop"></div>
    <div id="confirmModal" class="modal w-11/12 max-w-sm bg-gray-800 rounded-2xl shadow-2xl border border-gray-700 p-8 text-center">
        <h3 id="confirmModalTitle" class="text-xl font-bold text-white mb-4">هل أنت متأكد؟</h3>
        <p id="confirmModalMessage" class="text-gray-300 mb-8">لا يمكن التراجع عن هذا الإجراء.</p>
        <div class="flex justify-center gap-4">
            <button id="confirmCancelBtn" class="bg-gray-600 hover:bg-gray-500 text-white font-bold py-2 px-8 rounded-lg transition">إلغاء</button>
            <button id="confirmOkBtn" class="bg-red-600 hover:bg-red-700 text-white font-bold py-2 px-8 rounded-lg transition">تأكيد</button>
        </div>
    </div>

    <!-- Loading & Snackbar -->
    <div id="loading" class="fixed inset-0 bg-gray-900 bg-opacity-80 flex items-center justify-center z-50 hidden"><div class="animate-spin rounded-full h-12 w-12 border-t-2 border-b-2 border-cyan-500"></div></div>
    <div id="snackbar"></div>

    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-app.js";
        import { getAuth, signInAnonymously, signInWithCustomToken, onAuthStateChanged } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-auth.js";
        import { getFirestore, collection, addDoc, onSnapshot, doc, updateDoc, deleteDoc, query, where, serverTimestamp } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-firestore.js";

        const firebaseConfig = typeof __firebase_config !== 'undefined' ? JSON.parse(__firebase_config) : { apiKey: "YOUR_API_KEY", authDomain: "YOUR_AUTH_DOMAIN", projectId: "YOUR_PROJECT_ID" };
        const appId = typeof __app_id !== 'undefined' ? __app_id : 'my-media-tracker';
        
        const app = initializeApp(firebaseConfig);
        const db = getFirestore(app);
        const auth = getAuth(app);

        const CATEGORIES = ['روايات', 'مانجا/مانهوا', 'انمي', 'فيلم', 'مسلسل', 'كتاب', 'آخر'];
        const STATUSES = {
            watching: { text: 'جاري', color: 'bg-blue-500' },
            completed: { text: 'مكتمل', color: 'bg-green-500' },
            on_hold: { text: 'متوقف', color: 'bg-yellow-500' },
            dropped: { text: 'متروك', color: 'bg-red-500' },
            plan_to_watch: { text: 'للمشاهدة', color: 'bg-gray-500' }
        };
        let currentCategory = CATEGORIES[0];
        let userId = null;
        let unsubscribe = null;
        let allItems = []; // Cache for search functionality

        // --- UI ELEMENTS ---
        const loadingIndicator = document.getElementById('loading');
        const itemsGrid = document.getElementById('items-grid');
        const emptyState = document.getElementById('empty-state');
        const categoryTabsContainer = document.getElementById('category-tabs');
        const categoryTitle = document.getElementById('category-title');
        const searchInput = document.getElementById('searchInput');
        
        // Modals
        const addItemBtn = document.getElementById('addItemBtn');
        const itemModal = document.getElementById('itemModal');
        const itemModalBackdrop = document.getElementById('itemModalBackdrop');
        const closeModalBtn = document.getElementById('closeModalBtn');
        const itemForm = document.getElementById('itemForm');
        const modalTitle = document.getElementById('modal-title');
        const deleteItemBtn = document.getElementById('deleteItemBtn');
        const viewModal = document.getElementById('viewModal');
        const viewModalBackdrop = document.getElementById('viewModalBackdrop');
        const closeViewModalBtn = document.getElementById('closeViewModalBtn');
        const editItemBtn = document.getElementById('editItemBtn');
        const viewContent = document.getElementById('view-content');
        const confirmModal = document.getElementById('confirmModal');
        const confirmModalBackdrop = document.getElementById('confirmModalBackdrop');
        const confirmOkBtn = document.getElementById('confirmOkBtn');
        const confirmCancelBtn = document.getElementById('confirmCancelBtn');

        // --- AUTHENTICATION & INITIALIZATION ---
        // This listener reacts to any change in authentication state.
        onAuthStateChanged(auth, (user) => {
            if (user) {
                // If a user is detected and we haven't set up the UI yet, do it now.
                if (!userId) {
                    userId = user.uid;
                    initializeAppUI();
                }
            } else {
                // User is signed out.
                userId = null;
                console.log("User is signed out.");
            }
        });

        // This self-invoking async function handles the initial sign-in attempt.
        (async () => {
            try {
                // We only attempt to sign in if there's no currently authenticated user.
                if (!auth.currentUser) {
                    if (typeof __initial_auth_token !== 'undefined' && __initial_auth_token) {
                        await signInWithCustomToken(auth, __initial_auth_token);
                    } else {
                        await signInAnonymously(auth);
                    }
                } else {
                    // If a user already exists (e.g., from a previous session),
                    // trigger the UI initialization directly.
                    if (!userId) {
                       userId = auth.currentUser.uid;
                       initializeAppUI();
                    }
                }
            } catch (error) {
                console.error("Authentication failed:", error);
                // Provide a more helpful error message to the user.
                showError("فشل تسجيل الدخول. يرجى التأكد من تفعيل المصادقة المجهولة في إعدادات Firebase.");
            }
        })();

        // --- CORE APP LOGIC ---
        function initializeAppUI() {
            if (!userId) return;
            setupEventListeners();
            populateDropdowns();
            populateCategories();
            changeCategory(currentCategory);
        }

        function getCollectionRef() {
            return collection(db, `artifacts/${appId}/users/${userId}/mediaTracker`);
        }
        
        function setupEventListeners() {
            addItemBtn.addEventListener('click', openAddModal);
            closeModalBtn.addEventListener('click', closeModal);
            itemModalBackdrop.addEventListener('click', closeModal);
            itemForm.addEventListener('submit', handleFormSubmit);
            deleteItemBtn.addEventListener('click', handleDeleteItem);
            closeViewModalBtn.addEventListener('click', closeViewModal);
            viewModalBackdrop.addEventListener('click', closeViewModal);
            searchInput.addEventListener('input', () => renderItems(allItems));
            confirmCancelBtn.addEventListener('click', closeConfirmModal);
            confirmModalBackdrop.addEventListener('click', closeConfirmModal);
        }

        function populateDropdowns() {
            const categorySelect = document.getElementById('itemCategory');
            categorySelect.innerHTML = CATEGORIES.map(cat => `<option value="${cat}">${cat}</option>`).join('');
            
            const statusSelect = document.getElementById('itemStatus');
            statusSelect.innerHTML = Object.entries(STATUSES).map(([key, value]) => `<option value="${key}">${value.text}</option>`).join('');

            const ratingContainer = document.getElementById('itemRating');
            ratingContainer.innerHTML = '';
            for (let i = 10; i >= 1; i--) {
                const radio = document.createElement('input'); radio.type = 'radio'; radio.id = `star${i}`; radio.name = 'rating'; radio.value = i;
                const label = document.createElement('label'); label.htmlFor = `star${i}`; label.textContent = '★';
                ratingContainer.appendChild(radio); ratingContainer.appendChild(label);
            }
        }

        function populateCategories() {
            categoryTabsContainer.innerHTML = '';
            CATEGORIES.forEach(cat => {
                const tab = document.createElement('button');
                tab.textContent = cat;
                tab.dataset.category = cat;
                tab.className = 'px-4 py-2 text-sm font-medium rounded-md transition-colors duration-200';
                tab.classList.toggle('bg-cyan-500', cat === currentCategory);
                tab.classList.toggle('text-white', cat === currentCategory);
                tab.classList.toggle('text-gray-300', cat !== currentCategory);
                tab.classList.toggle('hover:bg-gray-700', cat !== currentCategory);
                tab.addEventListener('click', () => changeCategory(cat));
                categoryTabsContainer.appendChild(tab);
            });
        }

        function changeCategory(category) {
            currentCategory = category;
            categoryTitle.textContent = category;
            searchInput.value = '';
            
            const tabs = categoryTabsContainer.querySelectorAll('button');
            tabs.forEach(tab => {
                tab.classList.toggle('bg-cyan-500', tab.dataset.category === category);
                tab.classList.toggle('text-white', tab.dataset.category === category);
            });
            fetchAndRenderItems();
        }

        function fetchAndRenderItems() {
            showLoading();
            if (unsubscribe) unsubscribe();
            
            if (!userId) {
                hideLoading();
                showError("المستخدم غير مسجل دخوله.");
                return;
            }
            
            const itemsQuery = query(getCollectionRef(), where("category", "==", currentCategory));
            
            unsubscribe = onSnapshot(itemsQuery, (querySnapshot) => {
                allItems = [];
                querySnapshot.forEach((doc) => allItems.push({ id: doc.id, ...doc.data() }));
                allItems.sort((a, b) => (b.createdAt?.seconds || 0) - (a.createdAt?.seconds || 0));
                renderItems(allItems);
                hideLoading();
            }, (error) => {
                console.error("Error fetching items: ", error);
                showError("حدث خطأ في تحميل البيانات");
                hideLoading();
            });
        }

        function renderItems(items) {
            const searchTerm = searchInput.value.toLowerCase();
            const filteredItems = items.filter(item => item.name.toLowerCase().includes(searchTerm));

            itemsGrid.innerHTML = '';
            if (filteredItems.length === 0) {
                emptyState.classList.remove('hidden');
                itemsGrid.classList.add('hidden');
                emptyState.querySelector('h3').textContent = searchTerm ? 'لا توجد نتائج بحث' : 'هذا القسم فارغ حالياً';
            } else {
                emptyState.classList.add('hidden');
                itemsGrid.classList.remove('hidden');
                filteredItems.forEach(item => {
                    const card = document.createElement('div');
                    card.className = 'media-card bg-gray-800 rounded-lg shadow-lg overflow-hidden cursor-pointer flex flex-col';
                    card.addEventListener('click', () => openViewModal(item));
                    
                    const placeholderImg = `https://placehold.co/600x800/111827/475569?text=${encodeURIComponent(item.name)}`;
                    const statusInfo = STATUSES[item.status] || { text: '', color: 'bg-transparent' };

                    card.innerHTML = `
                        <div class="relative h-64">
                            <img src="${item.imageUrl || placeholderImg}" onerror="this.onerror=null;this.src='${placeholderImg}';" alt="${item.name}" class="w-full h-full object-cover">
                            <div class="absolute inset-0 bg-gradient-to-t from-gray-800 via-gray-800/40 to-transparent"></div>
                            ${item.status ? `<div class="status-badge ${statusInfo.color}">${statusInfo.text}</div>` : ''}
                            <div class="absolute bottom-0 p-4">
                                <h3 class="font-bold text-lg text-white truncate">${item.name}</h3>
                                <div class="flex items-center mt-1">
                                    ${Array(5).fill(0).map((_, i) => `<svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 ${i < (item.rating / 2) ? 'text-amber-400' : 'text-gray-600'}" viewBox="0 0 20 20" fill="currentColor"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z" /></svg>`).join('')}
                                </div>
                            </div>
                        </div>
                        <div class="bg-gray-700/50 p-3 text-center">
                            <p class="text-xs text-cyan-300 font-semibold truncate">${item.progress || 'لم يحدد التقدم'}</p>
                        </div>
                    `;
                    itemsGrid.appendChild(card);
                });
            }
        }

        // --- MODAL HANDLING ---
        function openModal() { itemModal.classList.add('show'); itemModalBackdrop.classList.add('show'); }
        function closeModal() {
            itemModal.classList.remove('show');
            itemModalBackdrop.classList.remove('show');
            itemForm.reset();
            document.getElementById('itemId').value = '';
            document.getElementById('moments-container').innerHTML = '';
            deleteItemBtn.classList.add('hidden');
        }
        function openAddModal() {
            itemForm.reset();
            document.getElementById('itemId').value = '';
            modalTitle.textContent = 'إضافة عمل جديد';
            deleteItemBtn.classList.add('hidden');
            document.getElementById('itemCategory').value = currentCategory;
            document.getElementById('moments-container').innerHTML = '';
            openModal();
        }
        function openEditModal(item) {
            closeViewModal();
            modalTitle.textContent = 'تعديل العمل';
            deleteItemBtn.classList.remove('hidden');
            document.getElementById('itemId').value = item.id;
            document.getElementById('itemName').value = item.name;
            document.getElementById('itemCategory').value = item.category;
            document.getElementById('itemStatus').value = item.status || 'watching';
            document.getElementById('itemImageUrl').value = item.imageUrl || '';
            document.getElementById('itemStory').value = item.story || '';
            document.getElementById('itemProgress').value = item.progress || '';
            if (item.rating) {
                const ratingRadio = document.querySelector(`#itemRating input[value="${item.rating}"]`);
                if(ratingRadio) ratingRadio.checked = true;
            }
            const momentsContainer = document.getElementById('moments-container');
            momentsContainer.innerHTML = '';
            if (item.importantMoments && Array.isArray(item.importantMoments)) {
                item.importantMoments.forEach(moment => addMomentField(moment.moment, moment.comment));
            }
            openModal();
        }
        function openViewModal(item) {
            const placeholderImg = `https://placehold.co/600x400/111827/475569?text=${encodeURIComponent(item.name)}`;
            viewContent.innerHTML = `
                <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                    <div class="md:col-span-1">
                        <img src="${item.imageUrl || placeholderImg}" onerror="this.onerror=null;this.src='${placeholderImg}';" alt="${item.name}" class="w-full h-auto object-cover rounded-lg shadow-lg">
                    </div>
                    <div class="md:col-span-2 space-y-4">
                        <h3 class="text-3xl font-bold text-cyan-400">${item.name}</h3>
                        <div class="flex items-center gap-2">${Array(10).fill(0).map((_, i) => `<span class="text-2xl ${i < item.rating ? 'text-amber-400' : 'text-gray-600'}">★</span>`).join('')}</div>
                        <p><strong>القسم:</strong> ${item.category}</p>
                        <p><strong>الحالة:</strong> ${STATUSES[item.status]?.text || 'غير محدد'}</p>
                        <p><strong>آخر فصل/حلقة:</strong> ${item.progress || 'لم يحدد'}</p>
                    </div>
                </div>
                <div><strong class="block mb-2">القصة:</strong><p class="bg-gray-900 p-3 rounded-lg whitespace-pre-wrap">${item.story || 'لا يوجد وصف.'}</p></div>
                ${item.importantMoments && item.importantMoments.length > 0 ? `<div><strong class="block mb-2">لحظات مهمة:</strong><ul class="list-none space-y-3">${item.importantMoments.map(m => `<li class="bg-gray-900 p-3 rounded-lg"><p class="font-semibold text-cyan-300">${m.moment}</p><p class="text-gray-400">${m.comment}</p></li>`).join('')}</ul></div>` : ''}`;
            editItemBtn.onclick = () => openEditModal(item);
            viewModal.classList.add('show');
            viewModalBackdrop.classList.add('show');
        }
        function closeViewModal() { viewModal.classList.remove('show'); viewModalBackdrop.classList.remove('show'); }

        function openConfirmModal(message, onConfirm) {
            document.getElementById('confirmModalMessage').textContent = message;
            confirmModal.classList.add('show');
            confirmModalBackdrop.classList.add('show');
            confirmOkBtn.onclick = () => {
                onConfirm();
                closeConfirmModal();
            };
        }
        function closeConfirmModal() {
            confirmModal.classList.remove('show');
            confirmModalBackdrop.classList.remove('show');
        }

        // --- FORM & DATA HANDLING ---
        async function handleFormSubmit(e) {
            e.preventDefault();
            const id = document.getElementById('itemId').value;
            const ratingInput = document.querySelector('#itemRating input:checked');
            const momentElements = document.getElementById('moments-container').querySelectorAll('.moment-entry');
            const importantMoments = Array.from(momentElements).map(el => ({ moment: el.querySelector('.moment-name').value, comment: el.querySelector('.moment-comment').value })).filter(m => m.moment);

            const itemData = {
                name: document.getElementById('itemName').value,
                category: document.getElementById('itemCategory').value,
                status: document.getElementById('itemStatus').value,
                imageUrl: document.getElementById('itemImageUrl').value,
                story: document.getElementById('itemStory').value,
                progress: document.getElementById('itemProgress').value,
                rating: ratingInput ? parseInt(ratingInput.value) : 0,
                importantMoments: importantMoments
            };

            try {
                if (id) { await updateDoc(doc(getCollectionRef(), id), itemData); } 
                else { itemData.createdAt = serverTimestamp(); await addDoc(getCollectionRef(), itemData); }
                closeModal();
            } catch (error) { console.error("Error saving item: ", error); showError("حدث خطأ أثناء حفظ البيانات"); }
        }
        function handleDeleteItem() {
            const id = document.getElementById('itemId').value;
            if (!id) return;
            openConfirmModal('هل أنت متأكد من رغبتك في حذف هذا العمل؟', async () => {
                try {
                    await deleteDoc(doc(getCollectionRef(), id));
                    closeModal();
                } catch (error) { console.error("Error deleting item: ", error); showError("حدث خطأ أثناء الحذف"); }
            });
        }

        // --- DYNAMIC FIELDS ---
        document.getElementById('addMomentBtn').addEventListener('click', () => addMomentField());
        function addMomentField(moment = '', comment = '') {
            const container = document.getElementById('moments-container');
            const div = document.createElement('div');
            div.className = 'moment-entry flex items-center gap-2';
            div.innerHTML = `<input type="text" class="moment-name w-1/3 bg-gray-600 border border-gray-500 rounded-lg px-2 py-1 text-sm" placeholder="الفصل/الدقيقة" value="${moment}"><input type="text" class="moment-comment w-2/3 bg-gray-600 border border-gray-500 rounded-lg px-2 py-1 text-sm" placeholder="تعليق..." value="${comment}"><button type="button" class="remove-moment-btn text-red-500 hover:text-red-400 p-1 rounded-full"><svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM7 9a1 1 0 000 2h6a1 1 0 100-2H7z" clip-rule="evenodd" /></svg></button>`;
            div.querySelector('.remove-moment-btn').addEventListener('click', () => div.remove());
            container.appendChild(div);
        }

        // --- UTILITY FUNCTIONS ---
        function showLoading() { loadingIndicator.classList.remove('hidden'); }
        function hideLoading() { loadingIndicator.classList.add('hidden'); }
        function showError(message) {
            const snackbar = document.getElementById("snackbar");
            snackbar.textContent = message;
            snackbar.className = "show";
            setTimeout(() => { snackbar.className = snackbar.className.replace("show", ""); }, 3000);
        }
    </script>
</body>
</html>

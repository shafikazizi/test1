<!doctype html>
<html lang="ms">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>eKenderaan - Sistem Pengurusan Kenderaan</title>
  <script src="/_sdk/data_sdk.js"></script>
  <script src="https://cdn.tailwindcss.com"></script>
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <style>
        body {
            box-sizing: border-box;
        }
        
        .fade-in {
            animation: fadeIn 0.3s ease-in;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .chart-container {
            position: relative;
            width: 100%;
            height: 300px;
        }
        
        @media (min-width: 768px) {
            .chart-container {
                height: 400px;
            }
        }
        
        .status-badge {
            display: inline-flex;
            align-items: center;
            padding: 0.25rem 0.75rem;
            border-radius: 9999px;
            font-size: 0.75rem;
            font-weight: 500;
        }
        
        .status-active { background-color: #d1fae5; color: #065f46; }
        .status-inactive { background-color: #fee2e2; color: #991b1b; }
        .status-pending { background-color: #fef3c7; color: #92400e; }
        .status-approved { background-color: #d1fae5; color: #065f46; }
        .status-rejected { background-color: #fee2e2; color: #991b1b; }
        .status-in-use { background-color: #dbeafe; color: #1e40af; }
        
        .spinner {
            border: 2px solid #f3f3f3;
            border-top: 2px solid #3498db;
            border-radius: 50%;
            width: 20px;
            height: 20px;
            animation: spin 1s linear infinite;
        }
        
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        @media print {
            .no-print { display: none !important; }
        }
    </style>
  <style>@view-transition { navigation: auto; }</style>
  <script src="/_sdk/element_sdk.js" type="text/javascript"></script>
 </head>
 <body class="bg-gradient-to-br from-blue-50 to-indigo-100 min-h-full"><!-- Login Section -->
  <div id="login-section" class="min-h-full flex items-center justify-center px-4 py-8">
   <div class="bg-white rounded-xl shadow-lg p-8 w-full max-w-md fade-in">
    <div class="text-center mb-8">
     <h1 class="text-3xl font-bold text-gray-800 mb-2">🚗 eKenderaan</h1>
     <p class="text-gray-600">Sistem Pengurusan Kenderaan</p>
     <p class="text-gray-600 text-sm">Pejabat Pendidikan Daerah Limbang</p>
    </div>
    <div class="flex mb-6 bg-gray-100 rounded-lg p-1"><button id="login-tab" class="flex-1 py-2 px-4 rounded-md font-medium transition-all bg-blue-600 text-white"> Log Masuk </button> <button id="register-tab" class="flex-1 py-2 px-4 rounded-md font-medium transition-all text-gray-600 hover:text-blue-600"> Daftar Akaun </button>
    </div>
    <div id="login-form-container">
     <form id="login-form" class="space-y-6">
      <div><label for="username" class="block text-sm font-medium text-gray-700 mb-2">Email Rasmi</label> <input type="email" id="username" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Masukkan email rasmi" required>
      </div>
      <div><label for="password" class="block text-sm font-medium text-gray-700 mb-2">Kata Laluan</label> <input type="password" id="password" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Masukkan kata laluan" required>
      </div><button type="submit" id="login-btn" class="w-full bg-blue-600 text-white py-3 px-6 rounded-lg font-medium hover:bg-blue-700 transition-colors"> 🔐 Log Masuk </button>
     </form>
     <div class="mt-6 p-4 bg-blue-50 rounded-lg border border-blue-200">
      <p class="text-sm text-blue-800 font-medium mb-2">ℹ️ Maklumat Penting</p>
      <p class="text-xs text-blue-700">Sistem ini menggunakan Canva Sheet untuk menyimpan data. Semua tempahan, pengguna, kenderaan dan pemandu akan disimpan secara automatik.</p>
      <p class="text-xs text-blue-700 mt-2"><strong>Admin:</strong> Daftar dengan nama "Shafik Azizi" untuk akses penuh.</p>
     </div>
    </div>
    <div id="register-form-container" class="hidden">
     <form id="register-form" class="space-y-6">
      <div><label for="reg-fullname" class="block text-sm font-medium text-gray-700 mb-2">Nama Penuh</label> <input type="text" id="reg-fullname" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Masukkan nama penuh" required>
      </div>
      <div><label for="reg-email" class="block text-sm font-medium text-gray-700 mb-2">Email Rasmi</label> <input type="email" id="reg-email" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="contoh@moe.gov.my" required>
      </div>
      <div><label for="reg-sector" class="block text-sm font-medium text-gray-700 mb-2">Sektor/Unit</label> <select id="reg-sector" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" required> <option value="">Pilih sektor/unit...</option> <option value="Sektor Perancangan">Sektor Perancangan</option> <option value="Sektor Pembelajaran">Sektor Pembelajaran</option> <option value="Sektor Pengurusan Sekolah">Sektor Pengurusan Sekolah</option> <option value="Sektor Pengurusan">Sektor Pengurusan</option> <option value="Sektor Pentaksiran dan Peperiksaan">Sektor Pentaksiran dan Peperiksaan</option> <option value="PTIS">PTIS</option> </select>
      </div>
      <div><label for="reg-password" class="block text-sm font-medium text-gray-700 mb-2">Kata Laluan</label> <input type="password" id="reg-password" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Cipta kata laluan" required>
      </div>
      <div><label for="reg-confirm-password" class="block text-sm font-medium text-gray-700 mb-2">Sahkan Kata Laluan</label> <input type="password" id="reg-confirm-password" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Sahkan kata laluan" required>
      </div><button type="submit" id="register-btn" class="w-full bg-green-600 text-white py-3 px-6 rounded-lg font-medium hover:bg-green-700 transition-colors"> ✅ Daftar Akaun </button>
     </form>
    </div>
    <div id="login-error" class="hidden mt-4 p-3 bg-red-100 border border-red-400 text-red-700 rounded-lg text-sm"></div>
    <div id="register-success" class="hidden mt-4 p-3 bg-green-100 border border-green-400 text-green-700 rounded-lg text-sm">
     ✅ Akaun berjaya didaftar! Sila log masuk.
    </div>
    <div id="register-error" class="hidden mt-4 p-3 bg-red-100 border border-red-400 text-red-700 rounded-lg text-sm"></div>
   </div>
  </div><!-- Main Application -->
  <div id="main-app" class="hidden px-4 py-8">
   <div class="container mx-auto max-w-7xl"><!-- Header -->
    <header class="mb-8">
     <div class="flex flex-col lg:flex-row justify-between items-center mb-4 gap-4">
      <div class="text-left">
       <p class="text-sm text-gray-600">Selamat datang,</p>
       <p id="current-user-display" class="font-semibold text-gray-800"></p>
       <p id="current-role-display" class="text-xs text-blue-600"></p>
      </div>
      <div class="text-center">
       <h1 class="text-4xl font-bold text-gray-800 mb-2">🚗 eKenderaan</h1>
       <p class="text-gray-600">Sistem Pengurusan Kenderaan</p>
       <p class="text-gray-600">Pejabat Pendidikan Daerah Limbang</p>
      </div><button id="logout-btn" class="px-4 py-2 bg-red-600 text-white rounded-lg hover:bg-red-700 transition-colors text-sm no-print"> 🚪 Log Keluar </button>
     </div>
    </header><!-- Navigation -->
    <nav class="mb-8 no-print">
     <div class="bg-white rounded-lg shadow-md p-2">
      <div class="flex flex-wrap gap-2 justify-center"><button id="tab-booking" class="px-4 py-2 rounded-md font-medium transition-all bg-blue-600 text-white">Tempahan</button> <button id="tab-tracking" class="px-4 py-2 rounded-md font-medium transition-all text-gray-600 hover:text-blue-600">Tracking</button> <button id="tab-schedule" class="px-4 py-2 rounded-md font-medium transition-all text-gray-600 hover:text-blue-600">Jadual</button> <button id="tab-history" class="px-4 py-2 rounded-md font-medium transition-all text-gray-600 hover:text-blue-600">Sejarah</button> <button id="tab-approval" class="px-4 py-2 rounded-md font-medium transition-all text-gray-600 hover:text-blue-600">Kelulusan</button> <button id="tab-users" class="px-4 py-2 rounded-md font-medium transition-all text-gray-600 hover:text-blue-600">Pengguna</button> <button id="tab-drivers" class="px-4 py-2 rounded-md font-medium transition-all text-gray-600 hover:text-blue-600">Pemandu</button> <button id="tab-vehicles" class="px-4 py-2 rounded-md font-medium transition-all text-gray-600 hover:text-blue-600">Kenderaan</button> <button id="tab-analytics" class="px-4 py-2 rounded-md font-medium transition-all text-gray-600 hover:text-blue-600">Analitik</button>
      </div>
     </div>
    </nav><!-- Booking Section -->
    <div id="booking-section" class="max-w-4xl mx-auto">
     <div class="bg-white rounded-xl shadow-lg p-8 fade-in">
      <h2 class="text-2xl font-bold text-gray-800 mb-6">📝 Borang Tempahan Kenderaan</h2>
      <form id="booking-form" class="space-y-6">
       <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
        <div><label for="employee-name" class="block text-sm font-medium text-gray-700 mb-2">Nama Pegawai</label> <input type="text" id="employee-name" class="w-full px-4 py-3 border border-gray-300 rounded-lg bg-gray-50" readonly>
        </div>
        <div><label for="employee-sector" class="block text-sm font-medium text-gray-700 mb-2">Sektor/Unit</label> <input type="text" id="employee-sector" class="w-full px-4 py-3 border border-gray-300 rounded-lg bg-gray-50" readonly>
        </div>
       </div>
       <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
        <div><label for="start-date" class="block text-sm font-medium text-gray-700 mb-2">Tarikh Mula</label> <input type="date" id="start-date" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500" required>
        </div>
        <div><label for="start-time" class="block text-sm font-medium text-gray-700 mb-2">Masa Mula</label> <input type="time" id="start-time" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500" required>
        </div>
       </div>
       <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
        <div><label for="end-date" class="block text-sm font-medium text-gray-700 mb-2">Tarikh Tamat</label> <input type="date" id="end-date" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500" required>
        </div>
        <div><label for="end-time" class="block text-sm font-medium text-gray-700 mb-2">Masa Tamat</label> <input type="time" id="end-time" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500" required>
        </div>
       </div>
       <div><label for="purpose" class="block text-sm font-medium text-gray-700 mb-2">Tujuan Penggunaan</label> <textarea id="purpose" rows="3" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500" placeholder="Nyatakan tujuan penggunaan..." required></textarea>
       </div><button type="submit" id="submit-booking-btn" class="w-full bg-blue-600 text-white py-3 px-6 rounded-lg font-medium hover:bg-blue-700 transition-colors"> 🚗 Hantar Tempahan </button>
      </form>
     </div>
    </div><!-- Tracking Section -->
    <div id="tracking-section" class="hidden">
     <div class="bg-white rounded-xl shadow-lg p-8 fade-in">
      <h2 class="text-2xl font-bold text-gray-800 mb-6">📍 Status Kenderaan</h2>
      <div id="car-status-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4"></div>
     </div>
    </div><!-- Schedule Section -->
    <div id="schedule-section" class="hidden">
     <div class="bg-white rounded-xl shadow-lg p-8 fade-in">
      <h2 class="text-2xl font-bold text-gray-800 mb-6">📅 Jadual Pinjaman</h2>
      <div id="schedule-content" class="overflow-x-auto">
       <p class="text-gray-500 text-center py-8">Tiada jadual pada masa ini</p>
      </div>
     </div>
    </div><!-- History Section -->
    <div id="history-section" class="hidden">
     <div class="bg-white rounded-xl shadow-lg p-8 fade-in">
      <h2 class="text-2xl font-bold text-gray-800 mb-6">📋 Sejarah Pinjaman</h2>
      <div class="overflow-x-auto">
       <table class="w-full">
        <thead>
         <tr class="bg-gray-50">
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Nama</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Kenderaan</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Tarikh</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Status</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Tujuan</th>
         </tr>
        </thead>
        <tbody id="history-table-body"></tbody>
       </table>
      </div>
     </div>
    </div><!-- Approval Section -->
    <div id="approval-section" class="hidden">
     <div class="bg-white rounded-xl shadow-lg p-8 fade-in">
      <h2 class="text-2xl font-bold text-gray-800 mb-6">✅ Kelulusan Tempahan</h2>
      <div class="overflow-x-auto">
       <table class="w-full">
        <thead>
         <tr class="bg-yellow-50">
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Nama</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Tarikh</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Tujuan</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700 no-print">Pilih Kenderaan</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700 no-print">Pilih Pemandu</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700 no-print">Tindakan</th>
         </tr>
        </thead>
        <tbody id="approval-table-body"></tbody>
       </table>
      </div>
     </div>
    </div><!-- Users Section -->
    <div id="users-section" class="hidden">
     <div class="bg-white rounded-xl shadow-lg p-8 fade-in">
      <h2 class="text-2xl font-bold text-gray-800 mb-6">👥 Pengurusan Pengguna</h2>
      <div class="overflow-x-auto">
       <table class="w-full">
        <thead>
         <tr class="bg-gray-50">
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Nama</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Email</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Sektor</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Peranan</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Status</th>
         </tr>
        </thead>
        <tbody id="users-table-body"></tbody>
       </table>
      </div>
     </div>
    </div><!-- Drivers Section -->
    <div id="drivers-section" class="hidden">
     <div class="bg-white rounded-xl shadow-lg p-8 fade-in">
      <h2 class="text-2xl font-bold text-gray-800 mb-6">🚗 Pengurusan Pemandu</h2>
      <div class="bg-gray-50 rounded-lg p-6 mb-6 no-print">
       <h3 class="text-lg font-semibold text-gray-800 mb-4">➕ Tambah Pemandu Baru</h3>
       <form id="add-driver-form" class="grid grid-cols-1 md:grid-cols-4 gap-4">
        <div><label for="driver-name" class="block text-sm font-medium text-gray-700 mb-2">Nama Pemandu</label> <input type="text" id="driver-name" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500" required>
        </div>
        <div><label for="driver-ic" class="block text-sm font-medium text-gray-700 mb-2">No. Kad Pengenalan</label> <input type="text" id="driver-ic" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500" required>
        </div>
        <div><label for="driver-license" class="block text-sm font-medium text-gray-700 mb-2">No. Lesen</label> <input type="text" id="driver-license" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500" required>
        </div>
        <div class="flex items-end"><button type="submit" id="add-driver-btn" class="w-full bg-blue-600 text-white py-2 px-4 rounded-lg hover:bg-blue-700 transition-colors"> ➕ Tambah </button>
        </div>
       </form>
      </div>
      <div class="overflow-x-auto">
       <table class="w-full">
        <thead>
         <tr class="bg-gray-50">
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Nama</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">No. K/P</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">No. Lesen</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Status</th>
         </tr>
        </thead>
        <tbody id="drivers-table-body"></tbody>
       </table>
      </div>
     </div>
    </div><!-- Vehicles Section -->
    <div id="vehicles-section" class="hidden">
     <div class="bg-white rounded-xl shadow-lg p-8 fade-in">
      <h2 class="text-2xl font-bold text-gray-800 mb-6">🚙 Pengurusan Kenderaan</h2>
      <div class="bg-gray-50 rounded-lg p-6 mb-6 no-print">
       <h3 class="text-lg font-semibold text-gray-800 mb-4">➕ Tambah Kenderaan Baru</h3>
       <form id="add-vehicle-form" class="grid grid-cols-1 md:grid-cols-5 gap-4">
        <div><label for="vehicle-brand" class="block text-sm font-medium text-gray-700 mb-2">Jenama</label> <select id="vehicle-brand" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500" required> <option value="">Pilih...</option> <option value="Toyota">Toyota</option> <option value="Honda">Honda</option> <option value="Perodua">Perodua</option> <option value="Proton">Proton</option> <option value="Nissan">Nissan</option> </select>
        </div>
        <div><label for="vehicle-model" class="block text-sm font-medium text-gray-700 mb-2">Model</label> <input type="text" id="vehicle-model" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500" required>
        </div>
        <div><label for="vehicle-plate" class="block text-sm font-medium text-gray-700 mb-2">No. Plat</label> <input type="text" id="vehicle-plate" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500" required>
        </div>
        <div><label for="vehicle-year" class="block text-sm font-medium text-gray-700 mb-2">Tahun</label> <select id="vehicle-year" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500" required> <option value="">Pilih...</option> <option value="2024">2024</option> <option value="2023">2023</option> <option value="2022">2022</option> <option value="2021">2021</option> <option value="2020">2020</option> </select>
        </div>
        <div class="flex items-end"><button type="submit" id="add-vehicle-btn" class="w-full bg-blue-600 text-white py-2 px-4 rounded-lg hover:bg-blue-700 transition-colors"> ➕ Tambah </button>
        </div>
       </form>
      </div>
      <div class="overflow-x-auto">
       <table class="w-full">
        <thead>
         <tr class="bg-gray-50">
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Kenderaan</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">No. Plat</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Tahun</th>
          <th class="px-4 py-3 text-left text-sm font-medium text-gray-700">Status</th>
         </tr>
        </thead>
        <tbody id="vehicles-table-body"></tbody>
       </table>
      </div>
     </div>
    </div><!-- Analytics Section -->
    <div id="analytics-section" class="hidden">
     <div class="bg-white rounded-xl shadow-lg p-8 fade-in">
      <h2 class="text-2xl font-bold text-gray-800 mb-6">📊 Analitik Penggunaan</h2>
      <div class="grid grid-cols-1 md:grid-cols-4 gap-4 mb-8">
       <div class="bg-gradient-to-r from-blue-500 to-blue-600 rounded-lg p-6 text-white">
        <p class="text-blue-100 text-sm">Jumlah Tempahan</p>
        <p id="total-bookings" class="text-2xl font-bold">0</p>
       </div>
       <div class="bg-gradient-to-r from-green-500 to-green-600 rounded-lg p-6 text-white">
        <p class="text-green-100 text-sm">Selesai</p>
        <p id="completed-bookings" class="text-2xl font-bold">0</p>
       </div>
       <div class="bg-gradient-to-r from-purple-500 to-purple-600 rounded-lg p-6 text-white">
        <p class="text-purple-100 text-sm">Paling Popular</p>
        <p id="most-popular" class="text-lg font-bold">-</p>
       </div>
       <div class="bg-gradient-to-r from-orange-500 to-orange-600 rounded-lg p-6 text-white">
        <p class="text-orange-100 text-sm">Menunggu</p>
        <p id="pending-bookings" class="text-2xl font-bold">0</p>
       </div>
      </div>
      <div class="chart-container mb-8">
       <canvas id="usage-chart"></canvas>
      </div>
     </div>
    </div><!-- Success Message -->
    <div id="success-message" class="hidden fixed top-4 right-4 bg-green-500 text-white px-6 py-4 rounded-lg shadow-lg z-50">
     ✅ Operasi berjaya!
    </div><!-- Loading Overlay -->
    <div id="loading-overlay" class="hidden fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50">
     <div class="bg-white rounded-lg p-6 flex items-center space-x-3">
      <div class="spinner"></div><span class="text-gray-700">Memproses...</span>
     </div>
    </div>
   </div>
  </div>
  <script>
        let currentUser = null;
        let allData = [];
        let usageChart = null;

        // Data Handler
        const dataHandler = {
            onDataChanged(data) {
                allData = data;
                updateAllViews();
            }
        };

        // Initialize Data SDK
        async function initializeApp() {
            const result = await window.dataSdk.init(dataHandler);
            if (!result.isOk) {
                console.error('Failed to initialize Data SDK');
            }
        }

        // Initialize on load
        initializeApp();

        // Helper functions
        function showLoading() {
            document.getElementById('loading-overlay').classList.remove('hidden');
        }

        function hideLoading() {
            document.getElementById('loading-overlay').classList.add('hidden');
        }

        function showSuccess(message = '✅ Operasi berjaya!') {
            const msg = document.getElementById('success-message');
            msg.textContent = message;
            msg.classList.remove('hidden');
            setTimeout(() => msg.classList.add('hidden'), 3000);
        }

        function showError(elementId, message) {
            const el = document.getElementById(elementId);
            el.textContent = message;
            el.classList.remove('hidden');
            setTimeout(() => el.classList.add('hidden'), 5000);
        }

        // Get data by type
        function getDataByType(type) {
            return allData.filter(item => item.type === type);
        }

        // Login/Register Toggle
        document.getElementById('login-tab').addEventListener('click', () => {
            document.getElementById('login-tab').classList.add('bg-blue-600', 'text-white');
            document.getElementById('login-tab').classList.remove('text-gray-600');
            document.getElementById('register-tab').classList.remove('bg-blue-600', 'text-white');
            document.getElementById('register-tab').classList.add('text-gray-600');
            document.getElementById('login-form-container').classList.remove('hidden');
            document.getElementById('register-form-container').classList.add('hidden');
        });

        document.getElementById('register-tab').addEventListener('click', () => {
            document.getElementById('register-tab').classList.add('bg-blue-600', 'text-white');
            document.getElementById('register-tab').classList.remove('text-gray-600');
            document.getElementById('login-tab').classList.remove('bg-blue-600', 'text-white');
            document.getElementById('login-tab').classList.add('text-gray-600');
            document.getElementById('register-form-container').classList.remove('hidden');
            document.getElementById('login-form-container').classList.add('hidden');
        });

        // Login
        document.getElementById('login-form').addEventListener('submit', async (e) => {
            e.preventDefault();
            showLoading();
            
            const email = document.getElementById('username').value;
            const password = document.getElementById('password').value;
            
            const users = getDataByType('user');
            const user = users.find(u => u.userEmail === email && u.userPassword === password);
            
            hideLoading();
            
            if (user) {
                currentUser = user;
                document.getElementById('login-section').classList.add('hidden');
                document.getElementById('main-app').classList.remove('hidden');
                document.getElementById('current-user-display').textContent = user.userName;
                document.getElementById('current-role-display').textContent = user.userRole;
                document.getElementById('employee-name').value = user.userName;
                document.getElementById('employee-sector').value = user.userSector;
                updateUI();
            } else {
                showError('login-error', '❌ Email atau kata laluan tidak sah!');
            }
        });

        // Register
        document.getElementById('register-form').addEventListener('submit', async (e) => {
            e.preventDefault();
            showLoading();
            
            const name = document.getElementById('reg-fullname').value;
            const email = document.getElementById('reg-email').value;
            const sector = document.getElementById('reg-sector').value;
            const password = document.getElementById('reg-password').value;
            const confirmPassword = document.getElementById('reg-confirm-password').value;
            
            if (password !== confirmPassword) {
                hideLoading();
                showError('register-error', '❌ Kata laluan tidak sepadan!');
                return;
            }
            
            const users = getDataByType('user');
            if (users.some(u => u.userEmail === email)) {
                hideLoading();
                showError('register-error', '❌ Email sudah digunakan!');
                return;
            }
            
            // Check if user is Shafik Azizi for admin role
            const userRole = (name === 'Shafik Azizi') ? 'Admin' : 'Pegawai';
            
            const result = await window.dataSdk.create({
                type: 'user',
                userId: Date.now().toString(),
                userName: name,
                userEmail: email,
                userSector: sector,
                userRole: userRole,
                userPassword: password,
                userStatus: 'Aktif',
                createdAt: new Date().toISOString(),
                bookingStartDate: null,
                bookingStartTime: null,
                bookingEndDate: null,
                bookingEndTime: null,
                bookingPurpose: null,
                bookingStatus: null,
                bookingVehicle: null,
                bookingDriver: null,
                bookingApprovedBy: null,
                bookingApprovedAt: null,
                vehicleBrand: null,
                vehicleModel: null,
                vehiclePlate: null,
                vehicleYear: null,
                vehicleStatus: null,
                driverName: null,
                driverIC: null,
                driverLicense: null,
                driverStatus: null
            });
            
            hideLoading();
            
            if (result.isOk) {
                document.getElementById('register-success').classList.remove('hidden');
                setTimeout(() => {
                    document.getElementById('register-success').classList.add('hidden');
                    document.getElementById('login-tab').click();
                }, 2000);
                document.getElementById('register-form').reset();
            } else {
                showError('register-error', '❌ Pendaftaran gagal. Sila cuba lagi.');
            }
        });

        // Logout
        document.getElementById('logout-btn').addEventListener('click', () => {
            currentUser = null;
            document.getElementById('main-app').classList.add('hidden');
            document.getElementById('login-section').classList.remove('hidden');
            document.getElementById('login-form').reset();
        });

        // Navigation
        const tabs = ['booking', 'tracking', 'schedule', 'history', 'approval', 'users', 'drivers', 'vehicles', 'analytics'];
        tabs.forEach(tab => {
            document.getElementById(`tab-${tab}`).addEventListener('click', () => {
                tabs.forEach(t => {
                    document.getElementById(`${t}-section`).classList.add('hidden');
                    document.getElementById(`tab-${t}`).classList.remove('bg-blue-600', 'text-white');
                    document.getElementById(`tab-${t}`).classList.add('text-gray-600');
                });
                document.getElementById(`${tab}-section`).classList.remove('hidden');
                document.getElementById(`tab-${tab}`).classList.add('bg-blue-600', 'text-white');
                document.getElementById(`tab-${tab}`).classList.remove('text-gray-600');
            });
        });

        // Booking Form
        document.getElementById('booking-form').addEventListener('submit', async (e) => {
            e.preventDefault();
            showLoading();
            
            const result = await window.dataSdk.create({
                type: 'booking',
                userId: currentUser.userId,
                userName: currentUser.userName,
                userEmail: currentUser.userEmail,
                userSector: currentUser.userSector,
                userRole: currentUser.userRole,
                userPassword: null,
                userStatus: null,
                bookingStartDate: document.getElementById('start-date').value,
                bookingStartTime: document.getElementById('start-time').value,
                bookingEndDate: document.getElementById('end-date').value,
                bookingEndTime: document.getElementById('end-time').value,
                bookingPurpose: document.getElementById('purpose').value,
                bookingStatus: 'Menunggu',
                bookingVehicle: null,
                bookingDriver: null,
                bookingApprovedBy: null,
                bookingApprovedAt: null,
                vehicleBrand: null,
                vehicleModel: null,
                vehiclePlate: null,
                vehicleYear: null,
                vehicleStatus: null,
                driverName: null,
                driverIC: null,
                driverLicense: null,
                driverStatus: null,
                createdAt: new Date().toISOString()
            });
            
            hideLoading();
            
            if (result.isOk) {
                document.getElementById('booking-form').reset();
                document.getElementById('employee-name').value = currentUser.userName;
                document.getElementById('employee-sector').value = currentUser.userSector;
                showSuccess('✅ Tempahan berjaya dihantar!');
            } else {
                showError('login-error', '❌ Tempahan gagal. Sila cuba lagi.');
            }
        });

        // Add Driver
        document.getElementById('add-driver-form').addEventListener('submit', async (e) => {
            e.preventDefault();
            showLoading();
            
            const result = await window.dataSdk.create({
                type: 'driver',
                userId: null,
                userName: null,
                userEmail: null,
                userSector: null,
                userRole: null,
                userPassword: null,
                userStatus: null,
                bookingStartDate: null,
                bookingStartTime: null,
                bookingEndDate: null,
                bookingEndTime: null,
                bookingPurpose: null,
                bookingStatus: null,
                bookingVehicle: null,
                bookingDriver: null,
                bookingApprovedBy: null,
                bookingApprovedAt: null,
                vehicleBrand: null,
                vehicleModel: null,
                vehiclePlate: null,
                vehicleYear: null,
                vehicleStatus: null,
                driverName: document.getElementById('driver-name').value,
                driverIC: document.getElementById('driver-ic').value,
                driverLicense: document.getElementById('driver-license').value,
                driverStatus: 'Aktif',
                createdAt: new Date().toISOString()
            });
            
            hideLoading();
            
            if (result.isOk) {
                document.getElementById('add-driver-form').reset();
                showSuccess('✅ Pemandu berjaya ditambah!');
            } else {
                showSuccess('❌ Gagal menambah pemandu');
            }
        });

        // Add Vehicle
        document.getElementById('add-vehicle-form').addEventListener('submit', async (e) => {
            e.preventDefault();
            showLoading();
            
            const result = await window.dataSdk.create({
                type: 'vehicle',
                userId: null,
                userName: null,
                userEmail: null,
                userSector: null,
                userRole: null,
                userPassword: null,
                userStatus: null,
                bookingStartDate: null,
                bookingStartTime: null,
                bookingEndDate: null,
                bookingEndTime: null,
                bookingPurpose: null,
                bookingStatus: null,
                bookingVehicle: null,
                bookingDriver: null,
                bookingApprovedBy: null,
                bookingApprovedAt: null,
                vehicleBrand: document.getElementById('vehicle-brand').value,
                vehicleModel: document.getElementById('vehicle-model').value,
                vehiclePlate: document.getElementById('vehicle-plate').value,
                vehicleYear: document.getElementById('vehicle-year').value,
                vehicleStatus: 'Tersedia',
                driverName: null,
                driverIC: null,
                driverLicense: null,
                driverStatus: null,
                createdAt: new Date().toISOString()
            });
            
            hideLoading();
            
            if (result.isOk) {
                document.getElementById('add-vehicle-form').reset();
                showSuccess('✅ Kenderaan berjaya ditambah!');
            } else {
                showSuccess('❌ Gagal menambah kenderaan');
            }
        });

        // Approve/Reject Booking
        window.approveBooking = async function(backendId, vehiclePlate, driverName) {
            const booking = allData.find(b => b.__backendId === backendId);
            if (!booking) return;
            
            if (!vehiclePlate || !driverName) {
                showSuccess('⚠️ Sila pilih kenderaan dan pemandu terlebih dahulu');
                return;
            }
            
            showLoading();
            
            const updated = {
                ...booking,
                bookingStatus: 'Diluluskan',
                bookingVehicle: vehiclePlate,
                bookingDriver: driverName,
                bookingApprovedBy: currentUser.userName,
                bookingApprovedAt: new Date().toISOString()
            };
            
            const result = await window.dataSdk.update(updated);
            hideLoading();
            
            if (result.isOk) {
                showSuccess('✅ Tempahan diluluskan!');
            } else {
                showSuccess('❌ Gagal meluluskan tempahan');
            }
        };

        window.rejectBooking = async function(backendId) {
            const booking = allData.find(b => b.__backendId === backendId);
            if (!booking) return;
            
            showLoading();
            
            const updated = {
                ...booking,
                bookingStatus: 'Ditolak',
                bookingApprovedBy: currentUser.userName,
                bookingApprovedAt: new Date().toISOString()
            };
            
            const result = await window.dataSdk.update(updated);
            hideLoading();
            
            if (result.isOk) {
                showSuccess('✅ Tempahan ditolak');
            } else {
                showSuccess('❌ Gagal menolak tempahan');
            }
        };

        // Update All Views
        function updateAllViews() {
            updateTracking();
            updateHistory();
            updateApproval();
            updateUsers();
            updateDrivers();
            updateVehicles();
            updateAnalytics();
        }

        function updateTracking() {
            const vehicles = getDataByType('vehicle');
            const bookings = getDataByType('booking');
            
            const grid = document.getElementById('car-status-grid');
            grid.innerHTML = vehicles.map(v => {
                const activeBooking = bookings.find(b => 
                    b.bookingVehicle === v.vehiclePlate && 
                    b.bookingStatus === 'Diluluskan' &&
                    new Date(b.bookingStartDate) <= new Date() &&
                    new Date(b.bookingEndDate) >= new Date()
                );
                
                const status = activeBooking ? 'Sedang Digunakan' : 'Tersedia';
                
                return `
                    <div class="bg-white border-2 border-gray-200 rounded-lg p-4">
                        <div class="text-2xl mb-2">🚗</div>
                        <h3 class="font-semibold text-gray-800">${v.vehicleBrand} ${v.vehicleModel}</h3>
                        <p class="text-sm text-gray-600">${v.vehiclePlate}</p>
                        <span class="status-badge ${status === 'Tersedia' ? 'status-active' : 'status-in-use'} mt-2">
                            ${status}
                        </span>
                        ${activeBooking ? `<p class="text-xs text-gray-500 mt-2">Dipinjam: ${activeBooking.userName}</p>` : ''}
                    </div>
                `;
            }).join('') || '<p class="text-gray-500 col-span-4 text-center py-8">Tiada kenderaan didaftarkan</p>';
        }

        function updateHistory() {
            const bookings = getDataByType('booking').filter(b => 
                b.bookingStatus === 'Diluluskan' || b.bookingStatus === 'Ditolak'
            );
            
            const tbody = document.getElementById('history-table-body');
            tbody.innerHTML = bookings.map(b => `
                <tr class="border-b hover:bg-gray-50">
                    <td class="px-4 py-3 text-sm">${b.userName}</td>
                    <td class="px-4 py-3 text-sm">${b.bookingVehicle || '-'}</td>
                    <td class="px-4 py-3 text-sm">${b.bookingStartDate}</td>
                    <td class="px-4 py-3 text-sm">
                        <span class="status-badge ${b.bookingStatus === 'Diluluskan' ? 'status-approved' : 'status-rejected'}">
                            ${b.bookingStatus}
                        </span>
                    </td>
                    <td class="px-4 py-3 text-sm">${b.bookingPurpose}</td>
                </tr>
            `).join('') || '<tr><td colspan="5" class="px-4 py-8 text-center text-gray-500">Tiada rekod</td></tr>';
        }

        function updateApproval() {
            const bookings = getDataByType('booking').filter(b => b.bookingStatus === 'Menunggu');
            const vehicles = getDataByType('vehicle');
            const drivers = getDataByType('driver');
            
            const tbody = document.getElementById('approval-table-body');
            tbody.innerHTML = bookings.map(b => `
                <tr class="border-b hover:bg-gray-50">
                    <td class="px-4 py-3 text-sm">${b.userName}</td>
                    <td class="px-4 py-3 text-sm">${b.bookingStartDate} ${b.bookingStartTime}</td>
                    <td class="px-4 py-3 text-sm">${b.bookingPurpose}</td>
                    <td class="px-4 py-3 text-sm no-print">
                        <select id="vehicle-${b.__backendId}" class="px-2 py-1 border rounded text-xs">
                            <option value="">Pilih kenderaan...</option>
                            ${vehicles.map(v => `<option value="${v.vehiclePlate}">${v.vehicleBrand} ${v.vehicleModel} (${v.vehiclePlate})</option>`).join('')}
                        </select>
                    </td>
                    <td class="px-4 py-3 text-sm no-print">
                        <select id="driver-${b.__backendId}" class="px-2 py-1 border rounded text-xs">
                            <option value="">Pilih pemandu...</option>
                            ${drivers.map(d => `<option value="${d.driverName}">${d.driverName}</option>`).join('')}
                        </select>
                    </td>
                    <td class="px-4 py-3 text-sm no-print">
                        <button onclick="approveBooking('${b.__backendId}', document.getElementById('vehicle-${b.__backendId}').value, document.getElementById('driver-${b.__backendId}').value)" class="px-3 py-1 bg-green-600 text-white rounded hover:bg-green-700 text-xs mr-2">
                            ✅ Lulus
                        </button>
                        <button onclick="rejectBooking('${b.__backendId}')" class="px-3 py-1 bg-red-600 text-white rounded hover:bg-red-700 text-xs">
                            ❌ Tolak
                        </button>
                    </td>
                </tr>
            `).join('') || '<tr><td colspan="6" class="px-4 py-8 text-center text-gray-500">Tiada tempahan menunggu kelulusan</td></tr>';
        }

        function updateUsers() {
            const users = getDataByType('user');
            const tbody = document.getElementById('users-table-body');
            tbody.innerHTML = users.map(u => `
                <tr class="border-b hover:bg-gray-50">
                    <td class="px-4 py-3 text-sm">${u.userName}</td>
                    <td class="px-4 py-3 text-sm">${u.userEmail}</td>
                    <td class="px-4 py-3 text-sm">${u.userSector}</td>
                    <td class="px-4 py-3 text-sm">${u.userRole}</td>
                    <td class="px-4 py-3 text-sm">
                        <span class="status-badge status-active">${u.userStatus}</span>
                    </td>
                </tr>
            `).join('') || '<tr><td colspan="5" class="px-4 py-8 text-center text-gray-500">Tiada pengguna</td></tr>';
        }

        function updateDrivers() {
            const drivers = getDataByType('driver');
            const tbody = document.getElementById('drivers-table-body');
            tbody.innerHTML = drivers.map(d => `
                <tr class="border-b hover:bg-gray-50">
                    <td class="px-4 py-3 text-sm">${d.driverName}</td>
                    <td class="px-4 py-3 text-sm">${d.driverIC}</td>
                    <td class="px-4 py-3 text-sm">${d.driverLicense}</td>
                    <td class="px-4 py-3 text-sm">
                        <span class="status-badge status-active">${d.driverStatus}</span>
                    </td>
                </tr>
            `).join('') || '<tr><td colspan="4" class="px-4 py-8 text-center text-gray-500">Tiada pemandu</td></tr>';
        }

        function updateVehicles() {
            const vehicles = getDataByType('vehicle');
            const tbody = document.getElementById('vehicles-table-body');
            tbody.innerHTML = vehicles.map(v => `
                <tr class="border-b hover:bg-gray-50">
                    <td class="px-4 py-3 text-sm">${v.vehicleBrand} ${v.vehicleModel}</td>
                    <td class="px-4 py-3 text-sm">${v.vehiclePlate}</td>
                    <td class="px-4 py-3 text-sm">${v.vehicleYear}</td>
                    <td class="px-4 py-3 text-sm">
                        <span class="status-badge status-active">${v.vehicleStatus}</span>
                    </td>
                </tr>
            `).join('') || '<tr><td colspan="4" class="px-4 py-8 text-center text-gray-500">Tiada kenderaan</td></tr>';
        }

        function updateAnalytics() {
            const bookings = getDataByType('booking');
            const pending = bookings.filter(b => b.bookingStatus === 'Menunggu');
            const completed = bookings.filter(b => b.bookingStatus === 'Diluluskan');
            
            document.getElementById('total-bookings').textContent = bookings.length;
            document.getElementById('completed-bookings').textContent = completed.length;
            document.getElementById('pending-bookings').textContent = pending.length;
            
            // Most popular vehicle
            const vehicleCount = {};
            completed.forEach(b => {
                if (b.bookingVehicle) {
                    vehicleCount[b.bookingVehicle] = (vehicleCount[b.bookingVehicle] || 0) + 1;
                }
            });
            
            const mostPopular = Object.keys(vehicleCount).length > 0 
                ? Object.keys(vehicleCount).reduce((a, b) => vehicleCount[a] > vehicleCount[b] ? a : b)
                : '-';
            
            document.getElementById('most-popular').textContent = mostPopular;
            
            // Chart
            const ctx = document.getElementById('usage-chart');
            if (ctx) {
                if (usageChart) {
                    usageChart.destroy();
                }
                
                const monthCounts = new Array(12).fill(0);
                bookings.forEach(b => {
                    if (b.bookingStartDate) {
                        const month = new Date(b.bookingStartDate).getMonth();
                        monthCounts[month]++;
                    }
                });
                
                usageChart = new Chart(ctx, {
                    type: 'bar',
                    data: {
                        labels: ['Jan', 'Feb', 'Mar', 'Apr', 'Mei', 'Jun', 'Jul', 'Ogos', 'Sep', 'Okt', 'Nov', 'Dis'],
                        datasets: [{
                            label: 'Tempahan',
                            data: monthCounts,
                            backgroundColor: '#3b82f6'
                        }]
                    },
                    options: {
                        responsive: true,
                        maintainAspectRatio: false,
                        scales: {
                            y: {
                                beginAtZero: true,
                                ticks: {
                                    stepSize: 1
                                }
                            }
                        }
                    }
                });
            }
        }

        function updateUI() {
            if (currentUser && (currentUser.userRole !== 'Admin' && currentUser.userRole !== 'Pengurus')) {
                document.getElementById('tab-approval').style.display = 'none';
                document.getElementById('tab-users').style.display = 'none';
                document.getElementById('tab-drivers').style.display = 'none';
                document.getElementById('tab-vehicles').style.display = 'none';
                document.getElementById('tab-analytics').style.display = 'none';
            }
        }
    </script>
 <script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9d9eb8af3104e41e',t:'MTc3MzEwNzk4MS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>

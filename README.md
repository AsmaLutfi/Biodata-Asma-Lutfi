<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title style="color:#bcbcbc;">Biodata</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; background-color: #e3148d; color: rgb(235, 120, 183); }
        .container { max-width: 600px; margin: auto; padding: 20px; border: 1px solid #de7aaf; border-radius: 10px; background-color: rgba(255, 255, 255, 0.9); color: black; }
        .hidden { display: none; }
        button { margin-top: 10px; padding: 10px; cursor: pointer; }
        img { width: 150px; height: 150px; border-radius: 50%; margin-bottom: 15px; }
    </style>
</head>
<body>
    <div class="container" id="page1">
        <h2>Halaman 1: Informasi Pribadi</h2>
        <img src="Picture 1.jpeg" widht="300" height="200" alt="Foto Profil">
        <p><strong>Nama:</strong> Asma Lutfi</p>
        <p><strong>Tempat & tanggal tahir:</strong> Siwalempu, 07 Mei 2005</p>
        <p><strong>Alamat:</strong> Jl. Lengaru, Palu Timur</p>
        <p><strong>Hobi:</strong> Gaming and Reading</p>
        <p><strong>Makanan Favorit:</strong> Es Krim</p>
        <p><strong>Minuman Favorit:</strong> Susu Strawberry</p>
        <p><strong>Musik Favorit:</strong> Blessing Cover by TNF</p>
        <button onclick="showPage(2)">Lanjut ke Halaman 2</button>
    </div>
    <div class="container hidden" id="page2">
    <h2>Halaman 2: Pendidikan & Keterampilan</h2>
    <img src="Universitas Tadulako.jpg" alt="Pendidikan">
    <p><strong>Universitas:</strong> Tadulako</p>
    <p><strong>Fakultas:</strong> Teknik</p>
    <p><strong>Prodi:</strong> S1 Sistem Informasi</p>
    <button onclick="showPage(1)">Kembali ke Halaman 1</button>
    </div>
    <script>
    function showPage(page) {
        document.getElementById('page1').classList.add('hidden');
        document.getElementById('page2').classList.add('hidden');
        document.getElementById('page' + page).classList.remove('hidden');
    }
    </script>
</body>
</html>

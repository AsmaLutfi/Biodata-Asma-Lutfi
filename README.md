<html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title style="color:#bcbcbc;">Biodata</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; background-color: #ff1ea1; color: white; }
        .container { max-width: 600px; margin: auto; padding: 20px; border: 1px solid #ee9bc5; border-radius: 10px; background-color: rgba(255, 255, 255, 0.9); color: black; }
        .hidden { display: none; }
        button { margin-top: 10px; padding: 10px; cursor: pointer; }
        img { width: 150px; height: 150px; border-radius: 50%; margin-bottom: 15px; }
    </style>
</head>
<body>
    <div class="container" id="content">
        <h2 id="title">Halaman 1: Informasi Pribadi</h2>
        <img id="image" src="profile.jpg" alt="Foto Profil">
        <p id="info1"><strong>Nama:</strong> Asma Lutfi</p>
        <p id="info2"><strong>Alamat:</strong> Jl. Lengaru, Palu</p>
        <p id="info3"><strong>Email:</strong> asmalutfi025@gmail.com</p>
        <p id="info4"><strong>No. HP:</strong> 082187937743</p>
        <button onclick="togglePage()" id="toggleButton">Lanjut ke Halaman 2</button>
    </div>
    <script>
    let page = 1;
    function togglePage() {
        if (page === 1) {
            document.getElementById('title').innerText = "Halaman 2: Pendidikan & Keterampilan";
            document.getElementById('image').src = "Universitas Tadulako.jpg";
            document.getElementById('image').alt = "Pendidikan";
            document.getElementById('info1').innerHTML = "<strong>Universitas:</strong> Tadulako";
            document.getElementById('info2').innerHTML = "<strong>Fakultas:</strong> Teknik";
            document.getElementById('info3').innerHTML = "<strong>Prodi:</strong> S1 Sistem Informasi";
            document.getElementById('info4').style.display = "none";
            document.getElementById('toggleButton').innerText = "Kembali ke Halaman 1";
            page = 2;
        } else {
            document.getElementById('title').innerText = "Halaman 1: Informasi Pribadi";
            document.getElementById('image').src = "profile.jpg";
            document.getElementById('image').alt = "Foto Profil";
            document.getElementById('info1').innerHTML = "<strong>Nama:</strong> Asma Lutfi";
            document.getElementById('info2').innerHTML = "<strong>Alamat:</strong> Jl. Lengaru, Palu";
            document.getElementById('info3').innerHTML = "<strong>Email:</strong> asmalutfi025@gmail.com";
            document.getElementById('info4').style.display = "block";
            document.getElementById('info4').innerHTML = "<strong>No. HP:</strong> 082187937743";
            document.getElementById('toggleButton').innerText = "Lanjut ke Halaman 2";
            page = 1;
        }
    }
    </script>
</body>
</html>

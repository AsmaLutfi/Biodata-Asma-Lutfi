<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Biodata</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; background-color: #cf12a6; color: rgb(231, 148, 213); }
        .container { max-width: 600px; margin: auto; padding: 20px; border: 1px solid #e383d3; border-radius: 10px; background-color: rgba(255, 255, 255, 0.9); color: black; }
        .hidden { display: none; }
        button { margin-top: 10px; padding: 10px; cursor: pointer; }
        img { width: 150px; height: 150px; border-radius: 50%; margin-bottom: 15px; }
    </style>
</head>
<body>
    <div class="container" id="content">
        <h2 id="title">Halaman 1: Informasi Pribadi</h2>
        <img id="image" src="Picture 1.jpeg" alt="Foto Profil">
        <p id="info1"><strong>Nama:</strong> Asma Lutfi</p>
        <p id="info2"><strong>Tempat & tanggal lahir:</strong> Siwalempu, 07 Mei 2005</p>
        <p id="info3"><strong>Alamat:</strong> Jl. Lengaru, Palu Timur</p>
        <p id="info4"><strong>Hobi:</strong> Gaming and Reading</p>
        <p id="info5"><strong>Makanan Favorit:</strong> Es Krim</p>
        <p id="info6"><strong>Minuman Favorit:</strong> Susu Strawberry</p>
        <p id="info7"><strong>Musik Favorit:</strong> Blessing Cover by TNF</p>
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
            document.getElementById('info3').innerHTML = "<strong>Program Studi:</strong> S1 Sistem Informasi";
            document.getElementById('info4').style.display = "none";
            document.getElementById('info5').style.display = "none";
            document.getElementById('info6').style.display = "none";
            document.getElementById('info7').style.display = "none";
            document.getElementById('toggleButton').innerText = "Kembali ke Halaman 1";
            page = 2;
        } else {
            document.getElementById('title').innerText = "Halaman 1: Informasi Pribadi";
            document.getElementById('image').src = "Picture 1.jpeg";
            document.getElementById('image').alt = "Foto Profil";
            document.getElementById('info1').innerHTML = "<strong>Nama:</strong> Asma Lutfi";
            document.getElementById('info2').innerHTML = "<strong>Tempat & tanggal lahir:</strong> Siwalempu, 07 Mei 2005";
            document.getElementById('info3').innerHTML = "<strong>Alamat:</strong> Jl. Lengaru, Palu Timur";
            document.getElementById('info4').style.display = "block";
            document.getElementById('info4').innerHTML = "<strong>Hobi:</strong> Gaming and Reading";
            document.getElementById('info5').style.display = "block";
            document.getElementById('info5').innerHTML = "<strong>Makanan Favorit:</strong> Es Krim";
            document.getElementById('info6').style.display = "block";
            document.getElementById('info6').innerHTML = "<strong>Minuman Favorit:</strong> Susu Strawberry";
            document.getElementById('info7').style.display = "block";
            document.getElementById('info7').innerHTML = "<strong>Musik Favorit:</strong> Blessing Cover by TNF";
            document.getElementById('toggleButton').innerText = "Lanjut ke Halaman 2";
            page = 1;
        }
    }
    </script>
</body>
</html>

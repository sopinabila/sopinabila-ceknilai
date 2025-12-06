<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cek Ganjil Genap</title>
</head>
<body>
    <h2>Program Cek Bilangan Ganjil Atau Genap</h2>

    <label for="angka">Maukkan Angka:</label>
    <input type="number" id="angka" placeholder="contoh: 7">
    <button onclick="cekAngka()">Cek</button>

    <p id="hasil"></p>

    <script>
        function cekAngka() {
            let angka = document.getElementById("angka").value;

            if (angka === "") {
                document.getElementById("hasil").innerHTML = "Harap masukkan angka!";
                return;
            }
            if (angka % 2 === 0) {
                document.getElementById("hasil").innerHTML = angka + "adalah bilangan genap.";
            } else {
                document.getElementById("hasil").innerHTML = angka + "adalah bilangan ganjil";
            }
        }
    </script>
</body>
</html>

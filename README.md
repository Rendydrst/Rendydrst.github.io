# Rendydrst.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Semangat UTS nya</title>
    <!-- Link CSS untuk Bootstrap 4 -->
    <link href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
    <!-- Link CSS untuk SweetAlert2 -->
    <link href="https://cdn.jsdelivr.net/npm/@sweetalert2/theme-dark@4/dark.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css" />
<style>
    body {
        background-image: url('Hh.jpg');
        /* Ganti URL gambar dengan URL gambar yang ingin digunakan */
        background-size: cover;
        background-position: center center;
        background-repeat: no-repeat;
        background-attachment: fixed;
        /* Menyebabkan gambar background tetap pada posisi fixed */
        background-color: rgba(0, 0, 0, 0.5);
        /* Mengatur transparansi background (0.5) */
    }
    .card-text {
        font-size: 16px; /* Ukuran teks standar */
    }

    /* Media query untuk mode tampilan ponsel */
    @media (max-width: 767px) {
      .card-text {
        font-size: 14px; /* Ukuran teks untuk mode tampilan ponsel */
      }
    }
</style>

</head>
<body>
<audio autoplay>
  <source src="bb.mp3" type="audio/mpeg">
</audio>

<audio id="myAudio" autoplay>
  <source src="bb.mp3" type="audio/mpeg">
</audio>

<div class="row mt-4 mb-4 mx-4">
    <div class="col-md-6 mx-auto">
        <h3 class="text-center mb-4"
            style="font-family: 'Helvetica', sans-serif; background: linear-gradient(45deg, #007bff, #00e6e6); -webkit-background-clip: text; color: transparent; text-transform: uppercase; letter-spacing: 2px; font-weight: bold;">
            Semangat UTS nya DUTHENG
        </h3>

        <div class="card shadow">
            <img class="card-img-top" src="a2.jpeg" alt="Card image cap">
            <div class="card-body ">
                <h5 class="card-title text-center" id="animated-text"></h5>
                <p class="card-text mt-2 mx-2" style="text-align: justify;">Semangat uts nya dutheng, maafin,cuman bisa bikin ginian aku gak jago coding soalnya hehe
                </p>
                <div class="card-body d-flex justify-content-center">
                    <button type="button" class="btn btn-primary text-center mx-auto" onclick="showSweetAlert()">Open</button>
                </div>
            </div>
        </div>
    </div>
</div>

    <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11/dist/sweetalert2.min.js"></script>
    <script>
    function showSweetAlert() {
        Swal.fire({
            title: '<span style="background: linear-gradient(45deg, #007bff, #00e6e6); -webkit-background-clip: text; font-size: 24px; font-weight: bold; color: transparent;">MAAF KALO AKU MASIH BANYAK KURANGNYA</span>', 
            html: '<div style="text-align: justify;">Soalnya kalo kamu tau, jujur kamu spesial</div>', 
            imageUrl: 'Bq.jpg', // Contoh URL gambar dari placeholder.com
            imageWidth: 400,
            imageHeight: 200,
            imageAlt: 'Custom image',
            background: '#FFFFFF',
            showClass: {
                popup: 'animate__animated animate__fadeInDown' // Menambahkan animasi fadeInDown dari Animate.css
            },
            hideClass: {
                popup: 'animate__animated animate__fadeOutDown' // Menambahkan animasi fadeOutDown dari Animate.css
            },
        }).then((result) => { // Menambahkan fungsi callback menggunakan then()
            if (result.isConfirmed) { // Menjalankan kode setelah mengklik tombol OK pada SweetAlert2
                setTimeout(function () {
                    Swal.fire({
                         title: '<span style="background: linear-gradient(45deg, #007bff, #00e6e6); -webkit-background-clip: text; font-size: 24px; font-weight: bold; color: transparent;">TERLALU TO THE POINT YGY </span>', 
                        html: '<div style="text-align: justify;">Gapapa lah sekali sekali aku juga wkwkwk, emang boleh se spesial itu</div>',
                        imageUrl: 'Uu.jpg', // Contoh URL gambar dari placeholder.com
                        imageWidth: 400,
                        imageHeight: 200,
                        imageAlt: 'Custom image',
                        background: '#FFFFFF',
                        showClass: {
                            popup: 'animate__animated animate__fadeInLeft' // Menambahkan animasi fadeInLeft dari Animate.css
                        },
                        hideClass: {
                            popup: 'animate__animated animate__fadeOutRight'
                        },
                    });
                }, 900); // Menunda Sweet Alert kedua selama 1 detik
            }
        });
    }
    </script>
<script>
    // JavaScript
    const text = "PASTI LANCAR SIH YAKIN AKU";
    const animatedText = document.getElementById("animated-text");
    let index = 0;
    let fontSize = 24; // Ukuran font awal (dalam piksel)

    function typeEffect() {
        if (index < text.length) {
            animatedText.textContent += text.charAt(index);
            index++;
            setTimeout(typeEffect, 100); // Waktu delay antara setiap karakter (ms)
        }

        // Cek mode tampilan pada perangkat mobile
        if (window.innerWidth <= 768) {
            // Ukuran font menjadi lebih kecil saat dalam mode tampilan pada perangkat mobile
            fontSize = 18; // Ukuran font pada mode mobile (dalam piksel)
        } else {
            fontSize = 24; // Ukuran font pada mode desktop (dalam piksel)
        }

        animatedText.style.fontSize = fontSize + "px"; // Set ukuran font pada element animatedText

        // Set warna latar belakang teks menjadi gradient linear
        animatedText.style.backgroundImage = "linear-gradient(45deg, #007bff, #00e6e6)";
        animatedText.style.webkitBackgroundClip = "text";
        animatedText.style.backgroundClip = "text";
        animatedText.style.color = "transparent"; // Set warna teks menjadi transparan
        animatedText.style.fontWeight = "bold"; // Set teks menjadi tebal
    }

    typeEffect();
</script>

<script>
  var audio = document.getElementById("myAudio");
  document.addEventListener("click", function() {
    audio.play();
  });
</script>


</body>
</html>

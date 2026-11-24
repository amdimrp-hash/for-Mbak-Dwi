<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Untuk Mbak Dwi ❤️</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    min-height: 100vh;
    font-family: 'Segoe UI', sans-serif;
    background: linear-gradient(135deg, #ffe0ec, #e4d5ff, #d6f1ff);
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 25px;
    overflow-x: hidden;
}

.card {
    background: rgba(255,255,255,0.85);
    max-width: 550px;
    width: 100%;
    padding: 35px 25px;
    border-radius: 25px;
    text-align: center;
    box-shadow: 0 15px 40px rgba(100,50,100,0.2);
    animation: muncul 1.2s ease;
}

@keyframes muncul {
    from {
        opacity: 0;
        transform: translateY(40px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.icon {
    font-size: 65px;
    margin-bottom: 15px;
    animation: goyang 2s infinite;
}

@keyframes goyang {
    0%,100% { transform: rotate(-5deg); }
    50% { transform: rotate(5deg); }
}

h1 {
    color: #d64d91;
    margin-bottom: 20px;
    font-size: 28px;
}

.message {
    color: #555;
    font-size: 16px;
    line-height: 1.9;
    text-align: justify;
    margin-bottom: 25px;
}

button {
    border: none;
    padding: 15px 25px;
    border-radius: 30px;
    background: linear-gradient(45deg, #ff70a6, #b77bff);
    color: white;
    font-size: 16px;
    font-weight: bold;
    cursor: pointer;
    transition: 0.3s;
    box-shadow: 0 5px 15px rgba(200,100,170,0.3);
}

button:hover {
    transform: scale(1.08);
}

#hasil {
    display: none;
    margin-top: 25px;
    color: #d64d91;
    font-size: 25px;
    font-weight: bold;
    animation: muncul 1s ease;
}

.footer {
    margin-top: 30px;
    color: #a45c91;
    font-style: italic;
    font-size: 15px;
}

.hati {
    position: fixed;
    top: -30px;
    animation: jatuh linear forwards;
    pointer-events: none;
}

@keyframes jatuh {
    to {
        transform: translateY(110vh) rotate(360deg);
        opacity: 0;
    }
}
</style>
</head>

<body>

<div class="card">

    <div class="icon">🌷</div>

    <h1>Selamat Hari Guru!</h1>

    <div class="message">
        mbak Dwi makasih ya udah mau jadi guruku
        kadang jikalau aku buat salah, atau menyakitkan
        hati mbak Dwi maaf ya mbak aku juga ga sengaja
        mungkin niatku bercanda namun bisa aja mbak Dwi
        sakit hati dengan candaan ku makasih ya mbak
        udah jadi guru tersabar di dunia makasih juga
        udah selalu ada ketika aku butuh bantuan
    </div>

    <button onclick="ucapan()">
        Klik untuk kejutan ❤️
    </button>

    <div id="hasil">
        🎉 Selamat Hari Guru Mbak Dwi! 🎉
        <p style="font-size:40px; margin-top:15px;">  
        </p>   
Mbak, terima kasih sudah menjadi guru yang sabar menghadapi segala tingkah lakuku. Terima kasih sudah mengajariku, bukan hanya tentang pelajaran, tetapi juga memberikan semangat ketika aku sedang menghadapi hari-hari yang sulit.
Maaf kalau selama belajar terkadang aku sulit diatur, banyak bertanya, atau membuat Mbak harus mengulang penjelasan berkali-kali.
Aku mungkin tidak selalu pandai mengungkapkan rasa terima kasih, tetapi aku benar-benar menghargai setiap waktu, kesabaran, dan kebaikan yang Mbak berikan.
Semoga Mbak selalu sehat, bahagia, dan tidak pernah kehilangan semangat untuk mengajar.
Selamat Hari Guru, Mbak. Terima kasih sudah menjadi bagian baik dalam perjalanan belajarku.💐❤️🌷

        Dari anak murid tercinta mbak Dwi (Rizki)
    </div>

</div>

<script>
function ucapan() {
    const hasil = document.getElementById("hasil");

    hasil.style.display = "block";

    document.querySelector("button").innerHTML =
        "Kejutan berhasil dibuka ❤️";
s
    for (let i = 0; i < 30; i++) {
        setTimeout(() => {
            const hati = document.createElement("div");

            hati.className = "hati";
            hati.innerHTML = ["❤️","💗","🌸","💖","🌷"][
                Math.floor(Math.random() * 5)
            ];

            hati.style.left = Math.random() * 100 + "vw";
            hati.style.animationDuration =
                (2 + Math.random() * 3) + "s";

            hati.style.fontSize =
                (15 + Math.random() * 20) + "px";

            document.body.appendChild(hati);

            setTimeout(() => hati.remove(), 5000);
        }, i * 100);
    }
}
</script>

</body>
</html>

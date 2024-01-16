<!DOCTYPE html>
<html lang="en">
<head>
   <link rel="icon" type="image/png" href="https://i.ibb.co/Xp1zYhD/1703575153-picsay.png">
  <center>
    <img src="https://i.ibb.co/yBz0myQ/images-1-removebg-preview-picsay.png"height="145px">
     <h1>~BOT HFT~</h1>
     <p>CREATED BY JHON</p>
  </center>
  <script>
document.getElementById('user-input').addEventListener('keypress', function (e) {
    if (e.key === 'Enter') {
        sendMessage();
    }
});

function sendMessage() {
    var userInput = document.getElementById('user-input');
    var chatContainer = document.getElementById('chat');

    var userMessage = userInput.value;
    if (!userMessage) return;

    appendMessage('user', userMessage, 'user-message');
    userInput.value = '';

    // cek respon bot 
    var botMessage = generateBotResponse(userMessage);
    appendMessage('bot', botMessage.message, botMessage.style);

    // SAYA DI SINI MENGGUNAKAN API GOOGLE
    var utterance = new SpeechSynthesisUtterance(botMessage.message);
    speechSynthesis.speak(utterance);
}

function generateBotResponse(userMessage) {
    var predefinedAnswers = {
      'lu lagi kenapa?':'gua lagi ga mod layanin kek gini!',
      'hallo mister botz':'hallo juga, ada apa?, ngajak berantem?,',
      'cara bujuk doi gimana?':'gitu aja gatau?, Samperin lah asu',
      'saya mau nanya':'apa?',
      'bejir':'diem kan lu!',
      'ko gua!':'halah berisik, Gua kick lu jadi author!',
      'ko gua?':'kan emang elu.',
      'ko ngegas!':'lu yang pertama mulai, bejir!',
      'biarin':'Sini sama gua, baku hantam.',
      'gatau':'kamu sehat?,mending turu, dek.',
      'awokawok':"malah ketawa bejir..", 
      'siapa jhon?':'jhon atau biasa di sebut Mister jhon,Dia adalah manusia, Dan Nama asli dia, Ade ikhsan nur Rahman Dia tinggal Di Tasikmalaya Tanggal lahir dia 26 april 2005,Dan dia sekarang Sekolah SMK Atau di sebut, Sekolah menengah kejuruan.',
        'hallo': 'Hallo juga, selamat datang, di website A.I Mister Jhon,apa ada yang saya bisa bantu?',
        'info pw': 'Password HFT yaitu Cybertasik jangan lupa Kapital semua',
        'terima kasih': 'sama sama senang berbincang bincang dengan anda jangan lupa support terus Mister Jhon','ada' : 'apa itu?',
        'Ada bang':'Apa itu? jangan macam macam!!','kepo' : 'bejir kamu berani sama saya?!!','pw nya apa' : 'kepo yaaa... awokaowk bercanda ngab.. jangan baper.. CYBERTASIK password nya, aduh, susah lagi bilang nya.','sc ddos':'dedeos-dedeos, dosa lu bang,... , yaudah lah nih tanggung sendiri ya, git clone https://github.com/Skyzz2/ECC-DDoS,jalanin sendiri ya','sc tools':'ini bree.. https://github.com/MR-JHONz/HFT-TOOLS, pasti pusing ya dengerin nya? hahhahaha ,Salin link nya aja ya','info':'Oke sedikit saya jelaskan ya, saya di buat oleh Mister jhon sejak Tanggal 28 desember 2023,jam 13.14, dia orang Suka tidur, tapi dia baik ko, Setia lagi.. hehe... jadi info jalanin nya gini pahami yaa... contoh : info password,sc tools, pengertian termux,commad termux,sc ddos,Mungkin segitu yang saya tau karna Bang Jhon ga ngasih tau dia pelit. Oh iya sebelum nya perkenalkan nama saya Mister Botz','pengertian termux ':'Termux adalah aplikasi terminal emulator yang dapat didownload secara gratis di platform Android dengan versi OS andorid versi 7 keatas. Dengan aplikasi Termux, pengguna dapat menjalankan perintah Linux dari perangkat Android yang digunakan.Aplikasi ini memberikan akses dengan tampilan command line (CLI) yang memungkinkan anda menjalankan perintah linux melalui perangkat android. Termux adalah aplikasi terminal emulator yang aman, dan juga memiliki fitur yang cukup lengkap.Dengan menggunakan termux, anda juga dapat melakukan aktivitas lain seperti pentesting atau pengujian keamanan pada sistem atau aplikasi di perangkat android yang digunakan. Hal tersebut bisa dilakukan karena pada termux mendukung installasi dan penggunaan tools keamanan, salah satunya nmap,haduhhh... cape..','command termux':'berupa script dengan perintah $ perl script_mu.pl atau $ ruby script_mu.rb atau $ python script_mu.pyMenggunakan Termux Untuk BekerjaMungkin kamu kesini belajar termux untuk hacking terutama untuk ngisengin orang ataupun berfikir untuk mbobol system,untuk orang profesional termux digunakan lebih dari itu.Saya sebagai IT admin sangat terbantu dengan adanya termux di HP android ku, saya bisa dengan mudah mengecek jaringan dan seluruh perangkat komputer yang ada di kantor pusat atau cabang menggunakan HP tanpa harus lama-lama menghidupkan laptop jika terjadi trouble.Menggunakan Termux Untuk Hacking Penggunaan komputer tidak terbatas begitu juga dengan termux,kamu bisa menggunakan nya sebagai tool atau platform untuk menjalankan aplikasi pentestool untuk kegiatan hacking.Ada beberapa hacking framework yang bisa kamu install dan gunakan untuk memudahkan dalam menemukan vulnerability ataupun membuat exploit. KESIMPULANTermux pada dasarnya linux yang bisa kamu manfaatkan untuk tujuan apapun,tak ada batasan penggunaan termux karena bergantung pada kreatifitas dan kebutuhan pemakainya,ingat termux hanyalah alat,beda orang beda cara dan tujuan dalam memakainya. Perlu diingat!! menggunakan termux tidak akan menjadikan mu punya skill hacking instan,karena untuk menjadi seorang hacker perlu belajar banyak hal dalam bidang komputer','kata kata nya dong om':'Hidup tidak berkewajiban memberikan apa yang kita harapkan.','terimakasih':'sama sama,senang bisa membantu kamu, jangan lupa support terus, Channel Mister Jhon yaa','oke':'baik terima kasih kembali','oke bang':'baik terima kasih kembali ya ','kamu siapa':'Saya adalah bot assitent Mister jhon , saya di buat untuk mempermudah kalian dalam mencari password tools','ohh':'iya bang','kamu itu siapa?':'aku adalah system bot pesan otomatis,buatan Mister jhon','ko ngegas':'hehe... bercanda ngabb.. jangan baperan.','kamu itu siapa':'saya adalah sebuah system operasi, saya di tugas kan untuk mempermudah kalian dalam mencari password tools dan mencari script tools nya.','iya':'iya apa, bang?','berani':'sini berantem sama gua!','berani lah':'sini sama gua berantem ayoo!','ayo':'samperin gua sini!','ayo siapa takut':'iya ayok sini',
    };

    var lowerCaseUserMessage = userMessage.toLowerCase();

    for (var key in predefinedAnswers) {
        if (lowerCaseUserMessage.includes(key)) {
            return {
                message: '' + predefinedAnswers[key],
                style: 'auto-reply-message'
            };
        }
    }

    // Default response if no predefined answer matches
    return {
        message: 'kata kunci tidak terdeteksi, sebelum nya minta maaf saya terbatas',
        style: 'bot-message'
    };
}

function appendMessage(sender, message, style) {
    var chatContainer = document.getElementById('chat');
    var messageDiv = document.createElement('div');
    messageDiv.textContent = message;
    messageDiv.className = style + ' ' + sender + '-message';
    chatContainer.appendChild(messageDiv);
}

  </script>
  <style>
  p {
    color:white;
  }
  body {
    background: black;
  }
#chat-container {
    max-width: 400px;
    margin: 50px auto;
    padding: 20px;
    border: 1px solid #ccc;
}

#chat {
    margin-bottom: 10px;
}

.user-message {
    background-color: #e6f7ff;
}

.bot-message {
    background-color: #f0f0f0;
    color: #333;
}

.auto-reply-message {
    background-color: #d9ffd9;
    font-style: italic;
}

#user-input {
    width: 70%;
    padding: 5px;
}

button {
    padding: 5px;
    cursor: pointer;
}
h1 {
  color: red;
  background:black;
}
/* Style dasar untuk tombol */
.music-button {
  display: inline-block;
  padding: 10px 20px;
  font-size: 16px;
  text-align: center;
  text-decoration: none;
  cursor: pointer;
  border: 2px solid #3498db;
  border-radius: 5px;
  color: #3498db;
  background-color: #fff;
}

/* Efek hover pada tombol */
.music-button:hover {
  background-color: #3498db;
  color: #fff;
}

/* Efek aktif ketika tombol ditekan */
.music-button:active {
  background-color: #2980b9;
  border-color: #2980b9;
  color: #fff;
}

  </style>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Auto-Reply Bot</title>
</head>
<body>
    <div id="chat-container">
        <div id="chat"></div>
        <input type="text" id="user-input" placeholder="Type your message...">
        <button onclick="sendMessage()">Send</button>
    </div>
    <script src="script.js"></script>
    <p><b>=> Sedikit info :</b><br>- Sebelum kalian menjalan kan BOT nya kalian ketik dulu <u><br><em>- Info</em><br></u><u>- Info pw</u><b> untuk mendapatkan password</b><br><em><u>-sc tools</u><b> TOOLS HFT</b><br><u><em>- sc ddos</em></u></em><b> TOOLS DDOS</b><br><b>=> Bot Mengandung suara</b><br><b>=> Cari di google untuk mencari lebih banyak informasi</b></p>
    <center>
     <a href="https://h.top4top.io/m_291866cp60.mp3" class="music-button">Putar Musik</a>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Google Search</title>
 <link rel="icon" type="image/png" href="favicon.ico">
    <style>
        }

        #search-container {
            text-align: center;
        }

        #search-box {
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            width: 300px;
            font-size: 16px;
        }

        #search-btn {
            padding: 10px 20px;
            background-color: #4285f4;
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
    </style>
</head>
<body>

<div id="search-container">
    <form action="https://www.google.com/search" method="GET" target="_blank">
        <input type="text" id="search-box" name="q" placeholder="Search on Google" required>
        <button type="submit" id="search-btn">Search</button>
    </form>
</div>

</body>
</html>

    </center>
</body>
</html>



<!DOCTYPE html>
<html lang="sq">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Kosova Skills</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #f2f2f2;
    }

    header {
      background-color: #004080;
      color: white;
      padding: 30px;
      text-align: center;
    }

    header h1 {
      margin: 0;
      font-size: 36px;
    }

    nav {
      background-color: #0066cc;
      padding: 10px 0;
    }

    .menyja ul {
      list-style: none;
      margin: 0;
      padding: 0;
      text-align: center;
    }

    .menyja ul li {
      display: inline-block;
      margin: 0 15px;
    }

    .menyja ul li a {
      color: white;
      text-decoration: none;
      font-weight: bold;
      padding: 10px 15px;
      transition: background 0.3s;
    }

    .menyja ul li a:hover {
      background-color: #003366;
      border-radius: 5px;
    }

    .logo img {
      width: 150px;
      border-radius: 50%;
    }

    #rreth_nesh {
      background-color: white;
      padding: 40px;
      text-align: center;
    }

    #rreth_nesh h1 {
      font-size: 28px;
      color: #333;
    }

    #rreth_nesh span {
      color: #004080;
    }

    #rreth_nesh p {
      font-size: 18px;
      color: #555;
    }

    .butoni {
      display: inline-block;
      margin-top: 15px;
      padding: 10px 25px;
      background-color: #004080;
      color: white;
      text-decoration: none;
      border-radius: 5px;
      cursor: pointer;
    }

    .butoni:hover {
      background-color: #002f5f;
    }

    .majtas {
      background-color: #fff;
      padding: 30px;
      margin: 20px;
      border-radius: 10px;
    }

    .majtas h2 {
      color: #004080;
    }

    footer {
      background-color: #004080;
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 30px;
    }

    footer a {
      color: #aaddff;
      text-decoration: none;
    }

    footer a:hover {
      text-decoration: underline;
    }

    /* Modal Styling */
    .modal {
      display: none; 
      position: fixed;
      z-index: 1;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      overflow: auto;
      background-color: rgba(0, 0, 0, 0.4);
    }

    .modal-content {
      background-color: #fff;
      margin: 15% auto;
      padding: 20px;
      border: 1px solid #888;
      width: 80%;
      max-width: 600px;
    }

    .modal-close {
      color: #aaa;
      float: right;
      font-size: 28px;
      font-weight: bold;
    }

    .modal-close:hover,
    .modal-close:focus {
      color: black;
      text-decoration: none;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <header>
    <h1>Kosova Skills</h1>
    <p>Ndërto të ardhmen me njohuri dhe aftësi të reja</p>
  </header>

  <!-- Menuja Kryesore -->
  <nav class="menyja">
    <ul>
      <li class="logo">
        <a href="index.html">
          <img src="kss.jpg" alt="Logo Kosova Skills">
        </a>
      </li>
      <li><a href="index.html">Ballina</a></li>
      <li><a href="informata.html">Informata</a></li>
      <li><a href="#linku">Linku</a></li>
      <li><a href="https://mustafa-ushtrime3.netlify.app/">Ushtrime3</a></li>
      <li><a href="#kontakti">Kontakti</a></li>
    </ul>
  </nav>

  <!-- Rreth Nesh -->
  <div id="rreth_nesh">
    <h1>Mësimi i <span>njohurive të reja</span> mund ta ndryshojë jetën</h1>
    <p>Ne kemi ndihmuar mijëra të rinj të zhvillohen profesionalisht. Zbulo më shumë se si mund të ndihmojmë edhe ty.</p>
    <button class="butoni" id="myBtn">Mëso më shumë</button>
  </div>

  <!-- Modal -->
  <div id="myModal" class="modal">
    <div class="modal-content">
      <span class="modal-close">&times;</span>
      <h2>Rreth Mësimit të Aftësive të Reja</h2>
      <p>Kosova Skills ofron mundësi të shkëlqyera për zhvillimin e aftësive teknike dhe profesionale për të rinjtë. Mësimet përfshijnë kurse praktike dhe teorike në fushat si:</p>
      <ul>
        <li>Programim dhe Zhvillim Software</li>
        <li>Menaxhim i Projekteve</li>
        <li>Marketing Digjital</li>
        <li>Design dhe UX/UI</li>
      </ul>
      <p>Pjesëmarrësit mund të zhvillojnë aftësi praktike, të marrin certifikata dhe të përfshihen në garat e zhvillimit profesional.</p>
    </div>
  </div>

  <!-- Informata -->
  <div class="majtas" id="linku">
    <h2>Informata</h2>
    <p>Kosova Skills është platformë edukative që promovon aftësi profesionale përmes punës praktike, mentorimit dhe garave në fusha të ndryshme teknike. Ne kemi ndihmuar miliona te rinje, e njeri nder te radhes mund te jesh edhe ti. Ne mundomi ne maksimum qe klienti te ndahet i kenaqur dhe me njohuri te reja, ky eshte qellimi i KosovaSkills. Shiko me shume se si mund te te ndihmojme</p>
  </div>

  <!-- Footer -->
  <footer id="kontakti">
    <p>&copy; 2025 Kosova Skills. Të gjitha të drejtat e rezervuara.</p>
    <p>Email: <a href="mailto:info@kosovaskills.org">info@kosovaskills.org</a> | Tel: +383 44 123 456</p>
    <p>
      <a href="#">Facebook</a> |
      <a href="#">Instagram</a> |
      <a href="#">LinkedIn</a>
    </p>
  </footer>

  <script>
    // Modal functionality
    var modal = document.getElementById("myModal");
    var btn = document.getElementById("myBtn");
    var span = document.getElementsByClassName("modal-close")[0];

    // When the user clicks the button, open the modal
    btn.onclick = function() {
      modal.style.display = "block";
    }

    // When the user clicks on <span> (x), close the modal
    span.onclick = function() {
      modal.style.display = "none";
    }

    // When the user clicks anywhere outside of the modal, close it
    window.onclick = function(event) {
      if (event.target == modal) {
        modal.style.display = "none";
      }
    }
  </script>

</body>
</html>


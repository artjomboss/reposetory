# reposetory
<<<<<<< HEAD
=======
<!DOCTYPE html>
<html lang="lv">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dvēseļu putenis</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            background: #f4f4f4;
        }

        header {
            background: #2c3e50;
            color: white;
            padding: 20px;
            text-align: center;
        }

        nav ul {
            list-style: none;
            padding: 0;
            margin: 10px 0 0;
        }

        nav ul li {
            display: inline;
            margin: 0 10px;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }

        nav a:hover {
            text-decoration: underline;
        }

        main {
            padding: 20px;
            text-align: center;
        }

        .book-cover {
            display: block;
            margin: 20px auto;
            width: 200px;
            cursor: pointer;
            transition: transform 0.3s;
        }

        .book-cover:hover {
            transform: scale(1.05);
        }

        section {
            background: white;
            margin: 20px auto;
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            max-width: 600px;
            overflow: hidden;
            max-height: 0;
            transition: max-height 0.5s ease, padding 0.5s ease;
        }

        section.open {
            max-height: 500px; /* pietiekami, lai saturu parādītu */
            padding: 15px;
        }

        footer {
            text-align: center;
            padding: 15px;
            background: #2c3e50;
            color: white;
        }

        /* Modal stils */
        .modal {
            display: none;
            position: fixed;
            z-index: 10;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background: rgba(0,0,0,0.7);
        }

        .modal-content {
            background: white;
            margin: 10% auto;
            padding: 20px;
            border-radius: 10px;
            width: 80%;
            max-width: 600px;
            text-align: left;
            position: relative;
        }

        .close-btn {
            position: absolute;
            top: 10px;
            right: 15px;
            font-size: 24px;
            font-weight: bold;
            cursor: pointer;
        }
    </style>
</head>
<body>

<header>
    <h1>Dvēseļu putenis</h1>
    <nav>
        <ul>
            <li><a href="#par-gramatu" onclick="openSection('par-gramatu')">Par grāmatu</a></li>
            <li><a href="#par-autoru" onclick="openSection('par-autoru')">Par autoru</a></li>
            <li><a href="#varoni" onclick="openSection('varoni')">Varoņi</a></li>
            <li><a href="#sizets" onclick="openSection('sizets')">Sižets</a></li>
            <li><a href="#atsauksme" onclick="openSection('atsauksme')">Atsauksme</a></li>
        </ul>
    </nav>
</header>

<main>

    <img src="https://upload.wikimedia.org/wikipedia/commons/5/5f/Dveselu_putenis.jpg" 
         alt="Dvēseļu putenis" 
         class="book-cover"
         onclick="openModal()">

    <section id="par-gramatu">
        <h2>Par grāmatu</h2>
        <p>Vēsturisks romāns par latviešu strēlniekiem Pirmajā pasaules karā.</p>
    </section>

    <section id="par-autoru">
        <h2>Par autoru</h2>
        <p>Aleksandrs Grīns bija latviešu rakstnieks un karavīrs.</p>
    </section>

    <section id="varoni">
        <h2>Galvenie varoņi</h2>
        <ul>
            <li>Artūrs Vanags</li>
            <li>Artūra tēvs</li>
            <li>Strēlnieki</li>
        </ul>
    </section>

    <section id="sizets">
        <h2>Sižets</h2>
        <p>Artūrs piedzīvo karu, zaudējumus un pieaug kā personība.</p>
    </section>

    <section id="atsauksme">
        <h2>Atsauksme</h2>
        <p>Ļoti emocionāla un svarīga grāmata par Latvijas vēsturi.</p>
    </section>

</main>

<footer>
    <p>&copy; 2026 Dvēseļu putenis</p>
</footer>

<!-- Modal -->
<div id="bookModal" class="modal">
    <div class="modal-content">
        <span class="close-btn" onclick="closeModal()">&times;</span>
        <h2>Dvēseļu putenis</h2>
        <p><strong>Par grāmatu:</strong> Vēsturisks romāns par latviešu strēlniekiem Pirmajā pasaules karā.</p>
        <p><strong>Par autoru:</strong> Aleksandrs Grīns bija latviešu rakstnieks un karavīrs.</p>
        <p><strong>Galvenie varoņi:</strong> Artūrs Vanags, Artūra tēvs, Strēlnieki</p>
        <p><strong>Sižets:</strong> Artūrs piedzīvo karu, zaudējumus un pieaug kā personība.</p>
        <p><strong>Atsauksme:</strong> Ļoti emocionāla un svarīga grāmata par Latvijas vēsturi.</p>
    </div>
</div>

<script>
    // Atver tikai vienu sadaļu
    function openSection(id) {
        let sections = document.querySelectorAll("section");
        sections.forEach(section => {
            if(section.id === id) {
                section.classList.toggle("open");
            } else {
                section.classList.remove("open");
            }
        });
    }

    // Modal funkcijas
    function openModal() {
        document.getElementById("bookModal").style.display = "block";
    }

    function closeModal() {
        document.getElementById("bookModal").style.display = "none";
    }

    // aizver modal, ja klikšķina ārpus tā
    window.onclick = function(event) {
        let modal = document.getElementById("bookModal");
        if(event.target === modal) {
            modal.style.display = "none";
        }
    }
</script>

</body>
</html>
>>>>>>> 4deaf4fddde6568e1d962a851c2c3c6c3f9c7d07

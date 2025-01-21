<!DOCTYPE html>
<html lang="sk">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Finančný agent UNIQA</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
            color: #333;
        }

        header {
            background-color: #0056a3;
            color: white;
            padding: 1rem;
            text-align: center;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #003d73;
            padding: 0.5rem;
        }

        nav a {
            color: white;
            margin: 0 1rem;
            text-decoration: none;
        }

        nav a:hover {
            text-decoration: underline;
        }

        main {
            padding: 2rem;
        }

        .contact {
            background-color: #e8f4fc;
            padding: 1rem;
            margin-top: 2rem;
            border-left: 5px solid #0056a3;
        }

        footer {
            text-align: center;
            padding: 1rem;
            background-color: #0056a3;
            color: white;
            margin-top: 2rem;
        }

        .languages {
            margin-top: 1rem;
        }
    </style>
    <script>
        const translations = {
            sk: {
                title: "Finančný agent UNIQA",
                about: "O nás",
                aboutText: "UNIQA je medzinárodná poisťovacia spoločnosť, ktorá ponúka širokú škálu finančných služieb. Usilujeme sa poskytnúť našim klientom pokoj a istotu do budúcnosti.",
                services: "Naše služby",
                service1: "Životné a zdravotné poistenie",
                service2: "Poistenie vozidiel",
                service3: "Majetkové poistenie",
                service4: "Finančné poradenstvo",
                contact: "Kontakty",
                phone: "Telefón",
                email: "Email",
                address: "Adresa",
                footer: "&copy; 2025 UNIQA. Všetky práva vyhradené.",
            },
            uk: {
                title: "Фінансовий агент UNIQA",
                about: "Про нас",
                aboutText: "UNIQA — це міжнародна страхова компанія, що надає широкий спектр фінансових послуг. Ми прагнемо забезпечити нашим клієнтам спокій та впевненість у майбутньому.",
                services: "Наші послуги",
                service1: "Страхування життя та здоров'я",
                service2: "Автострахування",
                service3: "Майнове страхування",
                service4: "Консультації з фінансових питань",
                contact: "Контакти",
                phone: "Телефон",
                email: "Email",
                address: "Адреса",
                footer: "&copy; 2025 UNIQA. Усі права захищено.",
            },
            en: {
                title: "UNIQA Financial Agent",
                about: "About Us",
                aboutText: "UNIQA is an international insurance company offering a wide range of financial services. We strive to provide our clients with peace of mind and confidence in the future.",
                services: "Our Services",
                service1: "Life and Health Insurance",
                service2: "Vehicle Insurance",
                service3: "Property Insurance",
                service4: "Financial Consulting",
                contact: "Contact Us",
                phone: "Phone",
                email: "Email",
                address: "Address",
                footer: "&copy; 2025 UNIQA. All rights reserved.",
            },
            cs: {
                title: "Finanční agent UNIQA",
                about: "O nás",
                aboutText: "UNIQA je mezinárodní pojišťovací společnost nabízející širokou škálu finančních služeb. Snažíme se našim klientům poskytnout klid a jistotu do budoucnosti.",
                services: "Naše služby",
                service1: "Životní a zdravotní pojištění",
                service2: "Pojištění vozidel",
                service3: "Majetkové pojištění",
                service4: "Finanční poradenství",
                contact: "Kontakty",
                phone: "Telefon",
                email: "Email",
                address: "Adresa",
                footer: "&copy; 2025 UNIQA. Všechna práva vyhrazena.",
            },
            hu: {
                title: "UNIQA Pénzügyi Ügynök",
                about: "Rólunk",
                aboutText: "Az UNIQA egy nemzetközi biztosítótársaság, amely széleskörű pénzügyi szolgáltatásokat kínál. Arra törekszünk, hogy ügyfeleink számára nyugalmat és jövőbeni biztonságot nyújtsunk.",
                services: "Szolgáltatásaink",
                service1: "Élet- és egészségbiztosítás",
                service2: "Járműbiztosítás",
                service3: "Ingatlanbiztosítás",
                service4: "Pénzügyi tanácsadás",
                contact: "Kapcsolat",
                phone: "Telefon",
                email: "Email",
                address: "Cím",
                footer: "&copy; 2025 UNIQA. Minden jog fenntartva.",
            }
        };

        function setLanguage(lang) {
            const elements = document.querySelectorAll("[data-translate]");
            elements.forEach(el => {
                const key = el.dataset.translate;
                el.textContent = translations[lang][key];
            });
            document.title = translations[lang].title;
        }
    </script>
</head>

<body onload="setLanguage('sk')">
    <header>
        <h1 data-translate="title">Finančný agent UNIQA</h1>
        <p data-translate="aboutText">UNIQA je medzinárodná poisťovacia spoločnosť...</p>
    </header>

    <nav>
        <a href="#about" data-translate="about">O nás</a>
        <a href="#services" data-translate="services">Naše služby</a>
        <a href="#contact" data-translate="contact">Kontakty</a>
    </nav>

    <main>
        <section id="about">
            <h2 data-translate="about">O nás</h2>
            <p data-translate="aboutText">UNIQA je medzinárodná poisťovacia spoločnosť...</p>
        </section>

        <section id="services">
            <h2 data-translate="services">Naše služby</h2>
            <ul>
                <li data-translate="service1">Životné a zdravotné poistenie</li>
                <li data-translate="service2">Poistenie vozidiel</li>
                <li data-translate="service3">Majetkové poistenie</li>
                <li data-translate="service4">Finančné poradenstvo</li>
            </ul>
        </section>

        <section id="contact" class="contact">
            <h2 data-translate="contact">Kontakty</h2>
            <p><span data-translate="phone">Telefón</span>: +421 951 826 628</p>
            <p><span data-translate="email">Email</span>: <a href="mailto:uniqa.alexmartysh@gmail.com">uniqa.alexmartysh@gmail.com</a></p>
            <p><span data-translate="address">Adresa</span>: Bratislava, Holičska 23</p>
        </section>

        <section class="languages">
            <h2>Meny jazykov</h2>
            <p>
                <button onclick="setLanguage('sk')">Slovenčina</button> |
                <button onclick="setLanguage('uk')">Українська</button> |
                <button onclick="setLanguage('en')">English</button> |
                <button onclick="setLanguage('hu')">Magyar</button> |
                <button onclick="setLanguage('cs')">Čeština</button>

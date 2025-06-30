<!DOCTYPE html>
<html lang="ro">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ghid Complet Interactiv - LiveHive BootCamp</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700;900&display=swap" rel="stylesheet">
    <style>
        html { scroll-behavior: smooth; }
        body { font-family: 'Inter', sans-serif; }
        .text-glow-yellow { text-shadow: 0 0 8px rgba(250, 204, 21, 0.7); }
        .text-glow-blue { text-shadow: 0 0 8px rgba(96, 165, 250, 0.7); }
        .text-glow-red { text-shadow: 0 0 8px rgba(239, 68, 68, 0.7); }
        .brand-yellow { color: #facc15; }
        .brand-blue { color: #60a5fa; }
        .brand-red { color: #f87171; }
        .brand-light { color: #e5e7eb; }
        
        table {
            border-collapse: collapse;
            width: 100%;
            margin-top: 1.5rem;
            margin-bottom: 1.5rem;
            font-size: 0.9em;
        }
        th, td {
            border: 1px solid #4b5563; /* gray-600 */
            padding: 12px;
            text-align: left;
            color: #d1d5db; /* gray-300 */
        }
        th {
            background-color: #1f2937; /* gray-800 */
            color: #facc15; /* brand-yellow */
            font-weight: 700;
        }
        
        /* Sidebar Navigation */
        .sidebar {
            position: fixed;
            top: 0;
            left: 0;
            height: 100vh;
            width: 280px;
            background-color: #111827;
            border-right: 1px solid #374151;
            padding: 2rem;
            overflow-y: auto;
            transform: translateX(-100%);
            transition: transform 0.3s ease-in-out;
            z-index: 40;
        }
        .sidebar.open { transform: translateX(0); }
        .sidebar a {
            display: block;
            padding: 0.75rem 1rem;
            color: #d1d5db;
            border-radius: 0.5rem;
            transition: background-color 0.2s, color 0.2s;
            font-weight: 500;
        }
        .sidebar a:hover, .sidebar a.active {
            background-color: #facc15;
            color: #1f2937; /* Dark gray, not black */
        }
        .sidebar .sub-link {
            padding-left: 2rem;
            font-size: 0.9em;
            color: #9ca3af;
        }
        
        .main-content {
            margin-left: 0;
            transition: margin-left 0.3s ease-in-out;
            width: 100%;
        }

        @media (min-width: 1024px) {
            .sidebar { transform: translateX(0); }
            .main-content { margin-left: 280px; }
            #menu-toggle { display: none; }
        }
        
        section {
            padding-top: 6rem;
            margin-top: -5rem;
        }
        h2.main-title {
            border-bottom: 2px solid #374151;
            padding-bottom: 0.5rem;
            margin-bottom: 1.5rem;
        }
        h3.sub-title {
            margin-top: 2rem;
            margin-bottom: 1rem;
        }
    </style>
</head>
<body class="bg-black text-brand-light">

    <!-- Sidebar Navigation -->
    <button id="menu-toggle" class="lg:hidden fixed top-4 left-4 z-50 p-2 rounded-md bg-gray-800 text-white">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
        </svg>
    </button>

    <nav id="sidebar" class="sidebar">
        <h2 class="text-2xl font-black brand-yellow text-glow-yellow mb-8 text-center">LiveHive<br>BootCamp</h2>
        <ul class="space-y-2">
            <li><a href="#capitolul_brand_personal">Brandul Personal</a></li>
            <li><a href="#capitolul_configurare_spatiu">Configurare Spațiu LIVE</a></li>
            <li><a href="#capitolul_intrare_live">Cum să Intri LIVE</a></li>
            <li><a href="#capitolul_interactiune">Interacțiunea cu Publicul</a></li>
            <li><a href="#capitolul_comunitate">Crearea Comunității</a></li>
        </ul>
    </nav>

    <!-- Main Content -->
    <div class="main-content">
        <header class="p-6 flex justify-center items-center sticky top-0 bg-black bg-opacity-80 backdrop-blur-sm z-30">
            <h1 class="text-2xl sm:text-4xl font-black text-center brand-yellow text-glow-yellow uppercase">Ghid Complet Creator</h1>
        </header>

        <main class="p-4 sm:p-8 md:p-12">
            <div class="max-w-5xl mx-auto">

                <!-- SECTION: Brandul Personal -->
                <section id="capitolul_brand_personal">
                    <h2 class="text-3xl font-bold brand-blue text-glow-blue main-title">Cum să Construiești un Brand Personal</h2>
                    <p class="text-lg leading-relaxed mb-6 text-gray-300">Cei mai de succes creatori LIVE captează atenția pentru că au un stil personal ieșit din comun. Procesul de găsire a stilului personal presupune trei pași-cheie: explorare, memorabilitate și rezonanță emoțională.</p>
                    
                    <h3 class="text-2xl font-bold brand-yellow sub-title">Ghid pentru Construirea Brandului</h3>
                     <ul class="list-disc list-inside mt-4 space-y-2 text-gray-300">
                        <li><strong class="text-brand-light">Explorează-te:</strong> Stilul personal derivă din autenticitate. Înțelege-ți mediul, educația, experiența și personalitatea. Acesta este fundamentul.</li>
                        <li><strong class="text-brand-light">Fii Memorabil:</strong> Ce te definește? Un aspect unic, un slogan, meme-uri? Amplifică aceste elemente pentru a deveni ușor de recunoscut.</li>
                        <li><strong class="text-brand-light">Creează Rezonanță Emoțională:</strong> Publicul se conectează cu atitudinile și valorile tale. Oferă o experiență pozitivă care declanșează emoții.</li>
                    </ul>

                    <h3 class="text-2xl font-bold brand-yellow sub-title">Optimizarea Profilului</h3>
                    <p class="text-gray-300">Profilul este cartea ta de vizită. Afișarea clară a aspectelor unice ajută utilizatorii să te înțeleagă rapid.</p>
                    <ul class="list-disc list-inside mt-4 space-y-2 text-gray-300">
                        <li><strong class="text-brand-light">Imagine de Profil:</strong> Clară, atractivă, reprezentativă pentru talentul tău.</li>
                        <li><strong class="text-brand-light">Pseudonim:</strong> Simplu, ușor de reținut, relevant.</li>
                        <li><strong class="text-brand-light">Biografie:</strong> Amplifică punctele forte și stilul unic. <strong class="brand-red">Include orele la care ești LIVE</strong>.</li>
                        <li><strong class="text-brand-light">Videoclipuri Fixate:</strong> Primele trei clipuri trebuie să arate clar stilul tău.</li>
                    </ul>
                </section>
                
                <!-- SECTION: Configurare Spațiu LIVE -->
                <section id="capitolul_configurare_spatiu">
                    <h2 class="text-3xl font-bold brand-blue text-glow-blue main-title">Cum să Configurezi un Spațiu pentru LIVE</h2>
                     <h3 class="text-2xl font-bold brand-yellow sub-title">Crearea unui LIVE Captivant</h3>
                     <p class="text-gray-300">Un spațiu optimizat îmbunătățește calitatea și experiența spectatorilor. Fundalul nu trebuie să fie dezordonat, iar sunetul trebuie să fie clar.</p>

                    <h3 class="text-2xl font-bold brand-yellow sub-title">Imaginea Creatorului</h3>
                    <p class="text-gray-300">Imaginea personală influențează prima impresie. Gestionează-ți stilul prin îmbrăcăminte, machiaj și expresii faciale.</p>
                     <ul class="list-disc list-inside mt-4 space-y-2 text-gray-300">
                        <li><strong class="text-brand-light">Îmbrăcăminte:</strong> Alege haine care se potrivesc stilului tău. Evită ținutele prea lejere. Accesoriile adaugă atractivitate.</li>
                        <li><strong class="text-brand-light">Machiaj și Coafură:</strong> Un aspect îngrijit, precis și elegant denotă profesionalism.</li>
                        <li><strong class="text-brand-light">Gestionarea Expresiilor:</strong> Fii expresiv și zâmbește! Exersează în oglindă pentru a-ți menține încrederea.</li>
                    </ul>

                     <h3 class="text-2xl font-bold brand-yellow sub-title">Iluminare și Fundal</h3>
                    <p class="text-gray-300">Iluminarea rezonabilă este mai importantă decât echipamentul. Fundalul trebuie să fie simplu și elegant.</p>
                     <ul class="list-disc list-inside mt-4 space-y-2 text-gray-300">
                        <li><strong class="text-brand-light">Filozofia Aspectului:</strong> Fundal simplu, elegant, care se potrivește stilului. Evită aglomerația și pereții albi.</li>
                        <li><strong class="text-brand-light">Logica Iluminării:</strong> O configurare bună include o <strong class="text-brand-yellow">lumină principală</strong> (pentru iluminare uniformă) și <strong class="text-brand-yellow">lumini de umplere</strong> (pentru a elimina umbrele și a crea contur).</li>
                        <li><strong class="text-brand-light">Lumini Decorative:</strong> Adaugă lumini ambientale (apus, neon) pentru atmosferă, dar cu moderație.</li>
                    </ul>
                </section>

                <!-- SECTION: Cum intri LIVE -->
                <section id="capitolul_intrare_live">
                    <h2 class="text-3xl font-bold brand-blue text-glow-blue main-title">Cum să Intri LIVE</h2>
                    
                    <h3 class="text-2xl font-bold brand-yellow sub-title">Partea 1: Pregătirea Scenei - Echipament</h3>
                    <p class="text-gray-300">Alegerea și utilizarea corectă a echipamentului hardware este fundamentală pentru un LIVE de calitate.</p>
                     <ul class="list-disc list-inside mt-4 space-y-2 text-gray-300">
                        <li><strong class="text-brand-light">Dispozitiv de Transmisiune:</strong> Se recomandă telefoane Apple recente sau, pentru calitate superioară (dans, exterior), aparate foto DSLR/Mirrorless.</li>
                        <li><strong class="text-brand-light">Configurația Computerului (pentru cameră):</strong> Procesor Intel i7 (gen 11+), Placă Video minim GTX 2060 (recomandat RTX 3060+), Memorie minim 16GB DDR4. Placa video este mai importantă decât procesorul.</li>
                        <li><strong class="text-brand-light">Echipament Audio:</strong> O placă de sunet și un microfon de calitate sunt decisive. Placa de sunet procesează semnalul audio și permite adăugarea de efecte.</li>
                     </ul>
                     <div class="overflow-x-auto">
                        <h4 class="text-xl font-semibold brand-blue mt-4">Recomandări Echipament Audio</h4>
                        <table>
                           <thead><tr><th>Nivel</th><th>Interfață / Mixer</th><th>Microfon</th><th>Avantaje</th></tr></thead>
                           <tbody>
                               <tr><td>Începător</td><td>Controler compact</td><td>Microfon fără fir compact</td><td>Simplu, complet, portabil, accesibil.</td></tr>
                               <tr><td>Intermediar</td><td>-</td><td>Microfon dinamic (ex: PodMic USB)</td><td>Calitate audio superioară, aspect profesional.</td></tr>
                               <tr><td>Avansat</td><td>Mixer profesional (ex: Caster Pro II)</td><td>Microfon de studio (ex: NT1-A)</td><td>Utilizare profesională, mai multe piste audio, efecte.</td></tr>
                           </tbody>
                        </table>
                    </div>

                    <h3 class="text-2xl font-bold brand-yellow sub-title">Partea 2: Intrarea LIVE pentru Prima Oară - Structura</h3>
                    <p class="text-gray-300">Un LIVE de succes este un LIVE planificat. Odată ce echipamentul este pregătit, urmează structura și conținutul.</p>
                     <ul class="list-disc list-inside mt-4 space-y-2 text-gray-300">
                        <li><strong class="text-brand-light">Program Consecvent:</strong> Un program fix ajută fanii să știe când să te urmărească.</li>
                        <li><strong class="text-brand-light">Videoclipuri Promoționale:</strong> Postarea de clipuri înainte de LIVE generează trafic și crește numărul de spectatori.</li>
                    </ul>
                     <div class="overflow-x-auto">
                        <h4 class="text-xl font-semibold brand-blue mt-4">Structura unui LIVE Atractiv</h4>
                        <table>
                            <thead><tr><th>Segment</th><th>Acțiuni Cheie</th><th>Pregătire</th></tr></thead>
                            <tbody class="text-gray-300">
                                <tr><td>Înainte de LIVE</td><td>Pregătire hardware, mediu de fundal, conținut.</td><td>Verifică echipamentul, setează scena.</td></tr>
                                <tr><td>Începerea LIVE-ului</td><td>Prezentare personală, spargerea gheții, previzualizare, muzică.</td><td>Pregătește o listă de redare și un script de prezentare.</td></tr>
                                <tr><td>Interacțiune</td><td>Organizare PK-uri, chat cu publicul, prezentare talente, dedicații.</td><td>Pregătește subiecte de discuție, jocuri pentru PK.</td></tr>
                                <tr><td>Menținerea Publicului</td><td>Folosirea funcțiilor (săculeți norocoși), interacțiune cu fanii de top.</td><td>Pregătește diamante pentru săculeți, scenarii pentru fani.</td></tr>
                                <tr><td>Încheierea LIVE-ului</td><td>Exprimarea recunoștinței, redarea unei piese de final, preview pentru următorul LIVE.</td><td>Alege o melodie de final, pregătește un teaser.</td></tr>
                            </tbody>
                        </table>
                    </div>
                </section>

                <!-- SECTION: Interacțiunea cu Publicul -->
                <section id="capitolul_interactiune">
                     <h2 class="text-3xl font-bold brand-blue text-glow-blue main-title">Cum să Păstrezi Spectatorii: Interacțiunea</h2>
                     <h3 class="text-2xl font-bold brand-yellow sub-title">Atitudini și Elemente Cheie</h3>
                     <p class="text-gray-300">Dacă un creator nu stăpânește cele patru elemente cheie ale interacțiunii, va pierde spectatorii. Pasivitatea și lipsa entuziasmului sunt greșeli comune.</p>
                     <div class="grid md:grid-cols-2 gap-8 text-gray-300">
                         <div>
                            <h4 class="text-xl font-semibold brand-blue mt-4">Patru Atitudini Esențiale</h4>
                             <ul class="list-disc list-inside space-y-2">
                                <li><strong class="text-brand-light">Atitudine Proactivă:</strong> Ia inițiativa, salută, împărtășește-ți povestea.</li>
                                <li><strong class="text-brand-light">Entuziasm:</strong> Un salut călduros și un ton prietenos cresc durata de vizionare.</li>
                                <li><strong class="text-brand-light">Politețe:</strong> Un zâmbet definește prima impresie. Fii civilizat și pozitiv.</li>
                                <li><strong class="text-brand-light">Respect:</strong> Privește spre cameră și arată respect tuturor, indiferent de nivelul lor.</li>
                             </ul>
                         </div>
                         <div>
                            <h4 class="text-xl font-semibold brand-blue mt-4">Patru Elemente de Bază ale LIVE-ului</h4>
                             <ul class="list-disc list-inside space-y-2">
                                <li><strong class="text-brand-light">Prezentare Personală:</strong> Spune cine ești, de unde ești, programul și tipul de conținut.</li>
                                <li><strong class="text-brand-light">Mesaje de Întâmpinare:</strong> Salută fiecare utilizator nou pe nume. Fii creativ bazat pe poza de profil (peisaj, anime, etc.).</li>
                                <li><strong class="text-brand-light">Mesaje de Mulțumire:</strong> Mulțumește personalizat, cu emoție (bucurie, gingășie), pentru fiecare cadou.</li>
                                <li><strong class="text-brand-light">Muzică de Fundal:</strong> Setează atmosfera cu liste de redare pentru diferite scenarii (început, chat, PK, etc.).</li>
                             </ul>
                         </div>
                    </div>
                </section>

                <!-- SECTION: Crearea Comunității -->
                <section id="capitolul_comunitate">
                    <h2 class="text-3xl font-bold brand-blue text-glow-blue main-title">Cum să Creezi și Menții Comunitatea de Fani</h2>
                    <p class="mb-6 text-gray-300">De ce sunt unii creatori atât de uniți cu fanii lor? Pentru că au construit și menținut activ o comunitate. Acest proces previne "migrarea" fanilor și încurajează loialitatea.</p>
                    
                     <h3 class="text-2xl font-bold brand-yellow sub-title">Principiile Menținerii Comunității</h3>
                     <ul class="list-disc list-inside mt-4 space-y-2 text-gray-300">
                        <li><strong class="brand-red">Fani de Nivel Înalt (Top Supporters):</strong> Necesită atenție specială. Înțelege-le preferințele. Calculează sumele din cadouri în contextul meciurilor PK pentru a evita cheltuieli excesive.</li>
                        <li><strong class="brand-yellow">Fani de Nivel Mediu (Top 10):</strong> Menține conexiunea prin saluturi și oferindu-le ocazional rolul de moderator.</li>
                        <li><strong class="brand-light">Fani Obișnuiți:</strong> Ei creează atmosfera dinamică. Încurajează-le interacțiunea.</li>
                    </ul>

                    <h3 class="text-2xl font-bold brand-yellow sub-title">Strategii Practice de Menținere</h3>
                    <ul class="list-disc list-inside space-y-3 text-gray-300">
                        <li><strong class="text-brand-light">Creează un Sentiment de Apartenență:</strong> Folosește un imn al camerei, dă fanilor loiali pseudonime, sărbătorește zilele lor de naștere.</li>
                        <li><strong class="text-brand-light">Menținerea Relației în Afara LIVE-ului:</strong> Creează grupuri de fani (fără condiții de intrare prea stricte), unde poți discuta subiecte diverse și oferi conținut exclusiv.</li>
                         <li><strong class="text-brand-light">Comunicare Personalizată:</strong> Răspunde la mesaje private. Trimite mulțumiri personalizate celor mai activi susținători (top 3) după fiecare LIVE.</li>
                        <li><strong class="text-brand-light">Distribuie Capturi de Ecran cu Cadouri:</strong> Arată-ți public recunoștința în grupurile de fani. Acest gest sincer consolidează legătura.</li>
                    </ul>
                </section>

            </div>
        </main>
    </div>

    <script>
        // --- Sidebar Navigation Script ---
        const menuToggle = document.getElementById('menu-toggle');
        const sidebar = document.getElementById('sidebar');

        menuToggle.addEventListener('click', (e) => {
            e.stopPropagation();
            sidebar.classList.toggle('open');
        });
        
        document.addEventListener('click', (event) => {
            if (window.innerWidth < 1024) {
                const isClickInsideSidebar = sidebar.contains(event.target);
                const isClickOnMenuToggle = menuToggle.contains(event.target);
                if (!isClickInsideSidebar && !isClickOnMenuToggle && sidebar.classList.contains('open')) {
                    sidebar.classList.remove('open');
                }
            }
        });
    </script>
</body>
</html>

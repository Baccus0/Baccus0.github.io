<!DOCTYPE html>

<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Brainf__k</title>

<style>
    * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
    }

    html {
        scroll-behavior: smooth;
    }

    body {
        font-family: Arial, Helvetica, sans-serif;
        background: #0d1117;
        color: #e6edf3;
        line-height: 1.6;
    }

    nav {
        position: sticky;
        top: 0;
        z-index: 100;
        background: #161b22;
        border-bottom: 1px solid #30363d;
        padding: 15px 8%;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    nav .logo {
        font-family: monospace;
        font-weight: bold;
        color: #58a6ff;
        font-size: 1.2rem;
    }

    nav a {
        color: #e6edf3;
        text-decoration: none;
        margin-left: 25px;
        font-size: 0.95rem;
    }

    nav a:hover {
        color: #58a6ff;
    }


    .hero {
        min-height: 90vh;
        display: flex;
        align-items: center;
        justify-content: center;
        text-align: center;
        padding: 50px 20px;
        background:
            radial-gradient(circle at center, #172554 0%, #0d1117 55%);
    }

    .hero-content {
        max-width: 850px;
    }

    .hero h1 {
        font-family: monospace;
        font-size: clamp(3rem, 9vw, 7rem);
        color: #58a6ff;
        letter-spacing: 5px;
        margin-bottom: 20px;
    }

    .hero h2 {
        font-size: clamp(1.4rem, 3vw, 2rem);
        margin-bottom: 20px;
    }

    .hero p {
        max-width: 700px;
        margin: auto;
        color: #8b949e;
        font-size: 1.1rem;
    }

    .hero-buttons {
        margin-top: 35px;
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        gap: 15px;
    }

    .button {
        display: inline-block;
        padding: 13px 22px;
        border: 1px solid #30363d;
        border-radius: 8px;
        background: #161b22;
        color: #e6edf3;
        text-decoration: none;
        transition: 0.2s;
    }

    .button:hover {
        background: #21262d;
        border-color: #58a6ff;
        transform: translateY(-2px);
    }

    .button.primary {
        background: #238636;
        border-color: #238636;
    }

    .button.primary:hover {
        background: #2ea043;
    }

    section {
        padding: 90px 8%;
    }

    section:nth-child(even) {
        background: #11161d;
    }

    .container {
        max-width: 1000px;
        margin: auto;
    }

    .section-title {
        font-size: 2.3rem;
        margin-bottom: 15px;
        color: #58a6ff;
    }

    .section-intro {
        color: #8b949e;
        margin-bottom: 35px;
        max-width: 800px;
    }

    .cards {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
        gap: 20px;
    }

    .card {
        background: #161b22;
        border: 1px solid #30363d;
        border-radius: 10px;
        padding: 25px;
    }

    .card h3 {
        color: #79c0ff;
        margin-bottom: 10px;
    }

    .card p {
        color: #8b949e;
    }

    pre {
        background: #010409;
        border: 1px solid #30363d;
        border-radius: 8px;
        padding: 20px;
        overflow-x: auto;
        margin: 20px 0;
    }

    code {
        font-family: "Courier New", monospace;
        color: #7ee787;
    }

    .command {
        font-family: monospace;
        font-size: 1.3rem;
        color: #ff7b72;
    }

    .command-table {
        width: 100%;
        border-collapse: collapse;
        margin-top: 30px;
    }

    .command-table th,
    .command-table td {
        border: 1px solid #30363d;
        padding: 13px;
        text-align: left;
    }

    .command-table th {
        background: #161b22;
        color: #79c0ff;
    }

    .command-table td:first-child {
        width: 100px;
        font-family: monospace;
        font-size: 1.2rem;
        color: #ff7b72;
    }

    .demo {
        background: #161b22;
        border: 1px solid #30363d;
        padding: 25px;
        border-radius: 10px;
        margin-top: 35px;
    }

    .demo button {
        margin: 5px;
        padding: 10px 15px;
        font-family: monospace;
        font-size: 1rem;
        cursor: pointer;
        border: 1px solid #30363d;
        border-radius: 6px;
        background: #0d1117;
        color: #e6edf3;
    }

    .demo button:hover {
        border-color: #58a6ff;
    }

    #demoOutput {
        margin-top: 20px;
        padding: 15px;
        min-height: 50px;
        background: #010409;
        border-radius: 6px;
        font-family: monospace;
        color: #7ee787;
    }

    .example {
        margin-bottom: 45px;
    }

    .example h3 {
        color: #79c0ff;
        margin-bottom: 10px;
    }

    .example p {
        color: #8b949e;
    }

    .sources li {
        margin: 12px 0;
    }

    .sources a {
        color: #58a6ff;
    }

    footer {
        text-align: center;
        padding: 35px;
        border-top: 1px solid #30363d;
        color: #8b949e;
    }

    @media (max-width: 700px) {
        nav {
            flex-direction: column;
            gap: 10px;
        }

        nav a {
            margin: 0 7px;
        }

        section {
            padding: 60px 6%;
        }
    }
</style>

</head>

<body>


<nav>
    <div class="logo">&gt;_ Brainf__k</div>

    <div>
        <a href="#origini">Origini</a>
        <a href="#come-funziona">Come funziona</a>
        <a href="#esempi">Esempi</a>
    </div>
</nav>

<header class="hero">

    <div class="hero-content">

        <h1>Brainf__k</h1>

        <h2>Otto comandi e un puntatore</h2>

        <p>
            Brainf__k è un linguaggio di programmazione esoterico
            progettato attorno a un'estrema semplicità. Possiede
            solamente otto comandi, ma è comunque completo secondo
            il modello di calcolo di Turing.
        </p>

        <div class="hero-buttons">

            <a class="button primary" href="#origini">
                Scopri le origini
            </a>

            <a class="button" href="#come-funziona">
                Come funziona?
            </a>

            <a class="button" href="#esempi">
                Guarda gli esempi
            </a>

        </div>

    </div>

</header>


<section>

    <div class="container">

        <h2 class="section-title">Cos'è Brainf__k?</h2>

        <p class="section-intro">
            Brainf__k è un linguaggio di programmazione esoterico
            creato da Urban Müller nel 1993. Il suo obiettivo era
            progettare un linguaggio estremamente minimale, con un
            compilatore il più piccolo possibile.
        </p>

        <div class="cards">

            <div class="card">
                <h3>8 comandi</h3>
                <p>
                    Il linguaggio riconosce solamente
                    <code>&gt; &lt; + - . , [ ]</code>.
                </p>
            </div>

            <div class="card">
                <h3>Completo secondo Turing</h3>
                <p>
                    Nonostante il suo insieme di istruzioni
                    minuscolo, Brainf__k può teoricamente eseguire
                    qualsiasi calcolo computabile.
                </p>
            </div>

            <div class="card">
                <h3>Esoterico</h3>
                <p>
                    Brainf__k è pensato soprattutto come curiosità,
                    esperimento e sfida di programmazione, non come
                    strumento pratico per sviluppare software.
                </p>
            </div>

            <div class="card">
                <h3>Minimalista</h3>
                <p>
                    Il linguaggio è stato progettato con l'obiettivo
                    di ottenere un compilatore estremamente piccolo.
                </p>
            </div>

        </div>

    </div>

</section>


<section id="origini">

    <div class="container">

        <h2 class="section-title">Origini</h2>

        <p class="section-intro">
            Brainf__k è stato creato dal programmatore svizzero
            Urban Müller nel 1993. Müller voleva creare un linguaggio
            di programmazione il cui compilatore fosse il più piccolo
            possibile.
        </p>

        <div class="cards">

            <div class="card">
                <h3>Ispirato a FALSE</h3>
                <p>
                    Müller prese ispirazione da FALSE, un linguaggio
                    di programmazione il cui compilatore occupava
                    soltanto 1024 byte.
                </p>
            </div>

            <div class="card">
                <h3>L'Amiga</h3>
                <p>
                    Il compilatore originale di Müller fu scritto
                    per Amiga utilizzando assembly Motorola 68000.
                </p>
            </div>

            <div class="card">
                <h3>Un compilatore minuscolo</h3>
                <p>
                    Il compilatore originale era incredibilmente
                    piccolo: una versione successiva occupava
                    solamente 240 byte.
                </p>
            </div>

            <div class="card">
                <h3>Una sfida</h3>
                <p>
                    La distribuzione originale includeva esempi
                    e sfidava i programmatori a dimostrare se fosse
                    possibile realizzare qualcosa di utile con
                    questo linguaggio.
                </p>
            </div>

        </div>

    </div>

</section>


<section id="come-funziona">

    <div class="container">

        <h2 class="section-title">Come funziona?</h2>

        <p class="section-intro">
            Possiamo immaginare Brainf__k come una lunga fila di
            celle di memoria e un puntatore che indica la cella
            attualmente utilizzata. All'inizio le celle contengono
            il valore zero.
        </p>

        <table class="command-table">

            <thead>
                <tr>
                    <th>Comando</th>
                    <th>Significato</th>
                </tr>
            </thead>

            <tbody>

                <tr>
                    <td>&gt;</td>
                    <td>
                        Sposta il puntatore di una cella verso destra.
                    </td>
                </tr>

                <tr>
                    <td>&lt;</td>
                    <td>
                        Sposta il puntatore di una cella verso sinistra.
                    </td>
                </tr>

                <tr>
                    <td>+</td>
                    <td>
                        Incrementa il valore della cella corrente.
                    </td>
                </tr>

                <tr>
                    <td>-</td>
                    <td>
                        Decrementa il valore della cella corrente.
                    </td>
                </tr>

                <tr>
                    <td>.</td>
                    <td>
                        Stampa il valore della cella corrente come
                        carattere.
                    </td>
                </tr>

                <tr>
                    <td>,</td>
                    <td>
                        Legge un carattere e lo inserisce nella cella
                        corrente.
                    </td>
                </tr>

                <tr>
                    <td>[</td>
                    <td>
                        Se la cella corrente vale zero, salta
                        all'istruzione dopo la parentesi quadra
                        corrispondente.
                    </td>
                </tr>

                <tr>
                    <td>]</td>
                    <td>
                        Se la cella corrente non vale zero, torna
                        alla parentesi quadra aperta corrispondente.
                    </td>
                </tr>

            </tbody>

        </table>


        <div class="demo">

            <h3>Prova gli otto comandi</h3>

            <p>
                I pulsanti mostrano in modo semplice come cambiano
                il puntatore e la cella di memoria corrente.
            </p>

            <button onclick="bfCommand('>')">&gt;</button>
            <button onclick="bfCommand('<')">&lt;</button>
            <button onclick="bfCommand('+')">+</button>
            <button onclick="bfCommand('-')">-</button>
            <button onclick="bfCommand('.')">.</button>

            <div id="demoOutput">
                Cella: 0 | Puntatore: 0 | Output:
            </div>

        </div>


        <h3 style="margin-top: 50px;">Un piccolo esempio</h3>

        <p>
            Il seguente programma Brainf__k incrementa la prima
            cella di memoria 65 volte e poi la stampa.
            Il valore ASCII 65 corrisponde alla lettera
            <strong>A</strong>.
        </p>

        <pre><code>+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++.</code></pre>

        <p>
            In un normale linguaggio di programmazione questa operazione
            sarebbe banale. In Brainf__k, persino stampare un singolo
            carattere può richiedere una lunga sequenza di operazioni.
        </p>

    </div>

</section>


<section id="esempi">

    <div class="container">

        <h2 class="section-title">Cosa è stato realizzato?</h2>

        <p class="section-intro">
            Brainf__k non è adatto allo sviluppo del normale software,
            ma nel corso degli anni i programmatori lo hanno utilizzato
            per realizzare esperimenti e programmi sorprendentemente
            complessi.
        </p>



        <div class="example">

            <h3>1. Hello World!</h3>

            <p>
                Uno degli esempi classici di Brainf__k è il programma
                "Hello World!", che stampa la famosa frase sullo schermo.
            </p>

            <pre><code>++++++++++[>+++++++>++++++++++>+++>+<<<<-]
```

>++.>+.+++++++..+++.>++.<<+++++++++++++++.>.
+++.------.--------.>+.>.</code></pre>

```
            <p>
                Questo esempio utilizza cicli, spostamenti del puntatore,
                operazioni aritmetiche e output, utilizzando solamente
                le istruzioni di Brainf__k.
            </p>

        </div>



        <div class="example">

            <h3>2. Gli esempi originali di Müller</h3>

            <p>
                La distribuzione originale di Brainf__k conteneva già
                programmi più complessi di un semplice "Hello World!",
                tra cui programmi per moltiplicazioni, divisioni,
                calcolo di numeri primi e altri piccoli strumenti.
            </p>

            <pre><code>src/
```

├── atoi.b
├── div10.b
├── hello.b
├── mul10.b
├── prime.b
└── varia.b</code></pre>

```
            <p>
                Questi programmi facevano parte della distribuzione
                originale di Urban Müller.
            </p>

        </div>



        <div class="example">

            <h3>3. I Quine</h3>

            <p>
                I programmatori di Brainf__k hanno realizzato anche
                dei <strong>quine</strong>: programmi capaci di stampare
                il proprio codice sorgente.
            </p>

            <p>
                Un quine è una sfida particolarmente interessante in
                un linguaggio minimalista come Brainf__k, perché il
                programma deve riprodurre le proprie istruzioni senza
                semplicemente leggere il proprio file sorgente.
            </p>

        </div>



        <div class="example">

            <h3>4. Programmi per l'insieme di Mandelbrot</h3>

            <p>
                Sono stati inoltre realizzati programmi Brainf__k capaci
                di calcolare e rappresentare l'insieme di Mandelbrot.
                Si tratta di esempi molto più ambiziosi, che dimostrano
                quanto lontano possa essere spinto il linguaggio.
            </p>

            <p>
                Il fatto che sia possibile implementare programmi di
                questo tipo in Brainf__k dimostra la potenza computazionale
                teorica del linguaggio, anche se scrivere programmi simili
                è estremamente complicato.
            </p>

        </div>



        <div class="card">

            <h3>Perché usarlo?</h3>

            <p>
                Principalmente per divertimento, sperimentazione e
                apprendimento. Brainf__k obbliga il programmatore a
                ragionare direttamente su memoria, puntatori, cicli
                e operazioni elementari.
            </p>

        </div>

    </div>

</section>


<section id="fonti">

    <div class="container sources">

        <h2 class="section-title">Fonti e approfondimenti</h2>

        <p class="section-intro">
            Le informazioni presenti in questa pagina sono state
            raccolte dalle seguenti fonti. Sono anche un buon punto
            di partenza per approfondire il linguaggio Brainf__k.
        </p>

        <ul>

            <li>
                <a href="https://www.Brainf__k.org/Brainf__k.html"
                   target="_blank">
                    Brainf__k.org — Yet Another Brainf__k Reference
                </a>
                — riferimento tecnico sul funzionamento del linguaggio.
            </li>

            <li>
                <a href="https://it.wikipedia.org/wiki/Brainf__k"
                   target="_blank">
                    Wikipedia Italia — Brainf__k
                </a>
                — panoramica storica e tecnica in italiano.
            </li>

            <li>
                <a href="https://esolangs.org/wiki/Brainf__k"
                   target="_blank">
                    Esolang Wiki — Brainf__k
                </a>
                — storia, istruzioni ed esempi del linguaggio.
            </li>

            <li>
                <a href="https://esolangs.org/wiki/Urban_M%C3%BCller/Tamedia_TX_2017_Transcript"
                   target="_blank">
                    Urban Müller — Tamedia TX 2017 Transcript
                </a>
                — testimonianza di Müller sulla creazione di Brainf__k.
            </li>

            <li>
                <a href="https://en.wikipedia.org/wiki/Brainf__k"
                   target="_blank">
                    Wikipedia — Brainf__k
                </a>
                — panoramica generale sulla storia e sul funzionamento.
            </li>

        </ul>

    </div>

</section>


<footer>

    <p>
        Creato per dimostrare l'eleganza meravigliosamente terribile
        di Brainf__k.
    </p>

    <p style="margin-top: 8px;">
        &lt; &gt; + - . , [ ]
    </p>

</footer>


<script>

    // Piccola dimostrazione interattiva del funzionamento
    // della memoria di Brainf__k.

    let memory = [0, 0, 0, 0, 0];
    let pointer = 0;
    let output = "";

    function bfCommand(command) {

        if (command === ">") {

            if (pointer < memory.length - 1) {
                pointer++;
            }

        }

        else if (command === "<") {

            if (pointer > 0) {
                pointer--;
            }

        }

        else if (command === "+") {

            memory[pointer]++;

            if (memory[pointer] > 255) {
                memory[pointer] = 0;
            }

        }

        else if (command === "-") {

            memory[pointer]--;

            if (memory[pointer] < 0) {
                memory[pointer] = 255;
            }

        }

        else if (command === ".") {

            output += String.fromCharCode(memory[pointer]);

        }

        document.getElementById("demoOutput").textContent =
            "Cella: " +
            memory[pointer] +
            " | Puntatore: " +
            pointer +
            " | Output: " +
            output;
    }

</script>
</body>
</html>

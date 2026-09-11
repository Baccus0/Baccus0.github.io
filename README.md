<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Brainfahh</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            background-color: #111827;
            color: #c1c1c1;
        }

        header {
            text-align: center;
            padding: 60px 20px;
            background: #172554;
        }

        header h1 {
            font-family: monospace;
            font-size: 60px;
            color: #58a6ff;
        }

        header p {
            font-size: 20px;
            color: #d1d5db;
        }

        nav {
            background-color: #1f2937;
            text-align: center;
            padding: 15px;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 15px;
        }

        nav a:hover {
            color: #58a6ff;
        }

        section {
            max-width: 900px;
            margin: auto;
            padding: 50px 20px;
        }

        h2 {
            color: #58a6ff;
        }

        .box {
            background-color: #1f2937;
            padding: 20px;
            margin-top: 20px;
            border-radius: 8px;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }

        th, td {
            border: 1px solid #4b5563;
            padding: 12px;
            text-align: left;
        }

        th {
            background-color: #374151;
        }

        td:first-child {
            font-family: monospace;
            font-size: 20px;
            color: #7ee787;
        }

        pre {
            background-color: #0b0f14;
            padding: 20px;
            overflow-x: auto;
            border-radius: 5px;
            color: #7ee787;
        }

        footer {
            text-align: center;
            padding: 25px;
            background-color: #1f2937;
            color: #9ca3af;
        }

        footer a {
            color: #58a6ff;
        }
    </style>
</head>

<body>

    <header>
        <h1>Brainf__k</h1>

        <p>
            Un linguaggio di programmazione esoterico e minimalista
        </p>
    </header>

    <nav>
        <a href="#home">Home</a>
        <a href="#origini">Origini</a>
        <a href="#funzionamento">Come funziona</a>
        <a href="#esempi">Esempi</a>
    </nav>


    <section id="home">

        <h2>Che cos'è Brainf__k?</h2>

        <p>
            Brainf__k è un linguaggio di programmazione esoterico creato
            da Urban Müller nel 1993.
        </p>

        <p>
            È famoso per la sua estrema semplicità: il linguaggio utilizza
            solamente otto comandi.
        </p>

        <div class="box">

            <h3>I suoi comandi sono:</h3>

            <p>
                <code>&gt; &lt; + - . , [ ]</code>
            </p>

            <p>
                Nonostante abbia pochissimi comandi, Brainf__k è
                Turing-completo, quindi può teoricamente eseguire
                qualsiasi tipo di calcolo.
            </p>

        </div>

    </section>


    <section id="origini">

        <h2>Le origini</h2>

        <p>
            Brainf__k è stato creato nel 1993 da
            <strong>Urban Müller</strong>.
        </p>

        <p>
            Müller voleva creare un linguaggio con un compilatore
            estremamente piccolo. Il progetto fu anche influenzato
            dal linguaggio FALSE.
        </p>

        <p>
            Il risultato fu un linguaggio composto da solamente otto
            istruzioni.
        </p>

    </section>


    <section id="funzionamento">

        <h2>Come funziona?</h2>

        <p>
            Brainf__k utilizza una serie di celle di memoria e un
            puntatore che indica la cella attualmente utilizzata.
        </p>

        <table>

            <tr>
                <th>Comando</th>
                <th>Funzione</th>
            </tr>

            <tr>
                <td>&gt;</td>
                <td>Sposta il puntatore a destra.</td>
            </tr>

            <tr>
                <td>&lt;</td>
                <td>Sposta il puntatore a sinistra.</td>
            </tr>

            <tr>
                <td>+</td>
                <td>Aumenta il valore della cella.</td>
            </tr>

            <tr>
                <td>-</td>
                <td>Diminuisce il valore della cella.</td>
            </tr>

            <tr>
                <td>.</td>
                <td>Stampa il carattere contenuto nella cella.</td>
            </tr>

            <tr>
                <td>,</td>
                <td>Inserisce un carattere nella cella.</td>
            </tr>

            <tr>
                <td>[</td>
                <td>Inizia un ciclo.</td>
            </tr>

            <tr>
                <td>]</td>
                <td>Termina il ciclo.</td>
            </tr>

        </table>

    </section>


    <section id="esempi">

        <h2>Esempi</h2>

        <h3>Hello World!</h3>

        <p>
            Uno degli esempi più conosciuti di Brainf__k è il programma
            "Hello World!", che stampa la frase sullo schermo.
        </p>

        <pre>
++++++++++[>+++++++>++++++++++>+++>+<<<<-]
>++.>+.+++++++..+++.>++.<<+++++++++++++++.>.+++.------.--------.>+.>.
        </pre>


        <div class="box">

            <h3>Altri programmi</h3>

            <p>
                Nel corso degli anni sono stati creati programmi
                Brainf__k molto più complessi, tra cui programmi per
                calcolare numeri primi, eseguire operazioni matematiche
                e persino programmi che producono il proprio codice.
            </p>

        </div>

    </section>


    <section>

        <h2>Fonti</h2>

        <ul>
            <li>
                <a href="https://www.brainfuck.org/brainfuck.html"
                   target="_blank">
                    Brainfuck.org
                </a>
            </li>

            <li>
                <a href="https://esolangs.org/wiki/Brainfuck"
                   target="_blank">
                    Esolang Wiki - Brainfuck
                </a>
            </li>

            <li>
                <a href="https://en.wikipedia.org/wiki/Brainfuck"
                   target="_blank">
                    Wikipedia - Brainfuck
                </a>
            </li>
        </ul>

    </section>


    <footer>
        Ciao
    </footer>

</body>
</html>

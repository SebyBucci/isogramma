# isogramma

Consegna:
Determina se una parola o una frase è un isogramma.

Per come lo intendiamo in questo esercizio, un isogramma è una parola o una frase che non ha lettere ripetute.
Sono ammessi spazi e segni di punteggiatura ripetuti.

Procedimento:
utilizziamo un array di interi di dimensione 26 per tenere traccia del numero di volte che ogni lettera dell'alfabeto compare nella stringa.
Per fare ciò, si utilizza un ciclo foreach per scorrere ogni carattere della stringa e si utilizza la funzione Char.IsLetter per verificare se il carattere è una lettera.
Se il carattere è una lettera, si incrementa il valore corrispondente dell'array di una unità e si controlla se il valore è maggiore di 1.
Se il valore è maggiore di 1, significa che la lettera è ripetuta nella stringa e il metodo restituisce "false". In caso contrario, il metodo continua a scorrere la stringa.

Se il metodo arriva alla fine della stringa senza trovare lettere ripetute, restituisce "true", indicando che la stringa è un isogramma.
Il metodo utilizza il metodo ToLower per convertire tutte le lettere in lettere minuscole, in modo che le lettere maiuscole e minuscole vengano trattate come uguali.

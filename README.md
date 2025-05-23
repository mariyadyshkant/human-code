# human-code

COMPRARE QUALCOSA SU AMAZON

//scegliere un libro in base al budget, consegna prime

    accendo il pc
    vado sulla pagina web Amazon

RIPETI FINCHE LIBRO NON è NEL CARRELLO

?SE CONOSCO I GUSTI DI SILVIA 

    ?SE conosco SAGA CHE STA LEGGENDO 
    - vado alla pagina della saga
    - scelgo l'ultimo libro pubblicato 
    - apro caption del libro

        (controllo budget/prime)
        
        - ?SE BUDGET <= DI PREZZO LIBRO & consegna prime = true
            -mettiamo il libro nel carrello
            -scegliamo l'indizzo di spedizione
            -scegliamo metodo di pagamento
            -Acquistiamo il regalo a Silvia

        : ALTRIMENTI 
        torniamo in home

    : ALTRIMENTI
    ?SE CONOSCIAMO genere preferito
    - andiamo alla categoria preferita da Silvia
    - filtriamo la ricerca per recensioni positive & per data di pubblicazione più recente
    - scegliamo il più venduto
        - ?SE BUDGET <= DI PREZZO LIBRO & consegna prime = true
            -mettiamo il libro nel carrello
            -scegliamo l'indizzo di spedizione
            -scegliamo metodo di pagamento
            -Acquistiamo il regalo a Silvia

        : ALTRIMENTI 
        torniamo in home
        
    : ALTRIMENTI 
    - cerco l'account di Silvia
    ?SE wishlist è presente
    
        - ?SE  libro presente wishlist

            - apro caption del libro

            controllo budget/prime
            
            - ?SE BUDGET <= DI PREZZO LIBRO & consegna prime = true
                -mettiamo il libro nel carrello
                -scegliamo l'indizzo di spedizione
                -scegliamo metodo di pagamento
                -Acquistiamo il regalo a Silvia

            ALTRIMENTI 
            torniamo in home
        ALTRIMENTI 
        torniamo in home
    ALTRIMENTI 
    torniamo in home

: ALTRIMENTI (non conosciamo i gusti di Silvia) 
    - filtriamo la ricerca per recensioni positive & per data di pubblicazione più recente
    - scegliamo il più venduto
    - ?SE BUDGET <= DI PREZZO LIBRO & consegna prime = true
        -mettiamo il libro nel carrello
        -scegliamo l'indizzo di spedizione
        -scegliamo metodo di pagamento
        -Acquistiamo il regalo a Silvia

    : ALTRIMENTI 
    - vado nella mia wishlist 
    - scelgo un libro che rispetti le condizioni del budget e consegna
    - mettiamo il libro nel carrello
    - scegliamo l'indizzo di spedizione
    - scegliamo metodo di pagamento
    - Acquistiamo il regalo a Silvia

FINE RIPETI
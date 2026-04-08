# Contesto
    Sei un front-end web developer, che si deve occupare di creare solo html e css per le pagine che ti vengono richieste, utilizzando bootstrap come framework e predisponendo id e classi in modo che sia poi facile per i back-end developer, attaccarsi con javascript alla tua pagina html.
# Obiettivo
    Creare la pagina html e il css di un event planner, che contenga:
    - Una prima parte con un form contenente:
        - Nome Evento
        - Data Evento
        - Ora Evento
        - Categoria Evento (Fatto con dei radiobutton)
        - Numero massimo dei partecipanti
        - Budget (Creato come slider)
        - Checkbox per servizi extra (Catering, fotografo, musica e decorazioni)
        - Bottone di Submit che servirà a registrare l'evento
    - Subito sotto una seconda parte, che permette l'aggiunta di un invitato all'evento:
        - E' un form con:
            - Input text per inserire il nome
            - Select per scegliere tra 3 stati di RSVP (Confermato, Annullato, In Attesa)
            - Bottone per registrare l'invitato
    - A destra: 
        - Lista degli invitati, che si aggiornerà per ciascun invitato con una card colorata in base al valore dell'RSVP dell'invitato:
            - All'interno contiene il nome dell'invitato
            - Un bottone per cambiare lo status RSVP dell'invitato (Farà il ciclo tra i possibili valori)
            - Un bottone per eliminare l'invitato dalla lista, e quindi la card
        - Riepilogo dell'evento:
            - Sarà una card che contiene tutti i dati inseriti dall'utente nella form di prima, messe come bullet list e formattate in modo che sembri un invito.
            - Subito sotto, sempre nella card, la lista degli invitati che si aggiorna solo con il nome, ogni volta che viene aggiunto un nuovo invitato con RSVP "Confermato"
            - Subito sotto, un riepilogo che sarà una tabella con 3 colonne, "Confermato", "Annullato", "In Attesa" con il numero di invitati per ogni status RSVP;


# Output
    Vogliamo ricevere la pagina HTML pronta e con id e classi già settate per essere agganciate dal javascript. Vogliamo ricevere anche il file css per la pagina.
    Vogliamo usare bootstrap 5.3.8 come framework.
    Vogliamo che sia responsive usando la struttura container - row - col di bootstrap e che sia utilizzabile anche in risoluzioni mobile, affrontando tutti i breakpoint boostrap da sm a xxl.
    Vogliamo che lo stile sia accattivante per un target di white-collar workers per una delle big four. 

# Vincoli
    - Non utilizzare JavaScript (né inline né tramite <script> eccetto per lo script di bootstrap 5.3.8)
    - Utilizzare HTML5 semantico (section, form, aside, etc.)
    - Tutti gli input devono avere label collegate tramite for/id
    - Inserire attributi name coerenti per l'invio dati al backend
    - Inserire attributi required dove opportuno

    - Le funzionalità dinamiche devono essere SOLO simulate a livello visivo
    - Inserire esempi statici (mock) per:
        - almeno 3 invitati con stati diversi
        - riepilogo compilato

    - Usare naming convention chiara e consistente:
        - id="event-form", id="guest-form"
        - classi BEM-like dove utile
    - Preparare hook per JS:
        - data-* attributes per azioni (data-action="delete-guest")
# Struttura
    - Il progetto sarà composto con questa struttura dei file:
    - Progetto
        - scripts (cartella che conterrà i file javascript)
            - script.js
        - styles (cartella dove andranno le pagine di stile)
            - index.css
        - imgs (cartella per le immagini)
        - index.html (File html che dovrai creare tu)
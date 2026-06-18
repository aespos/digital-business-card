# Digital Business Card — Alessandro Esposito

Mini landing page statica, mobile-first e senza dipendenze esterne, pronta per
essere pubblicata gratuitamente con GitHub Pages e usata come destinazione di
un QR Code o di un pass Apple Wallet.

## Struttura

```text
digital-business-card/
├── index.html
├── style.css
├── README.md
├── alessandro-esposito.vcf
└── assets/
    ├── alessandro-esposito-profile.jpg
    ├── company-logo.png
    └── alessandro-esposito-qr.png
```

## Personalizzare foto, logo e QR Code

Inserire nella cartella `assets`:

- la foto profilo con nome `alessandro-esposito-profile.jpg`;
- il logo aziendale con nome `company-logo.png`;
- il QR Code con nome `alessandro-esposito-qr.png`.

Per sostituire un'immagine mantenendo lo stesso formato, è sufficiente
sovrascrivere il file corrispondente. Se si cambia nome o formato, aggiornare
anche il relativo attributo `src` in `index.html`.

La foto profilo dovrebbe essere quadrata e di buona qualità. Per il logo è
preferibile un PNG con sfondo trasparente. Il QR Code deve avere un buon
contrasto, margine bianco e dimensioni consigliate di almeno 600 × 600 pixel.

## Generare il QR Code

1. Pubblicare prima il sito su GitHub Pages.
2. Copiare l'URL pubblico, per esempio:
   `https://NOME-UTENTE.github.io/digital-business-card/`.
3. Usare un generatore QR affidabile per creare un QR Code di tipo URL.
4. Impostare come contenuto l'URL completo della landing page.
5. Esportare il QR Code in PNG e salvarlo come
   `assets/alessandro-esposito-qr.png`.
6. Caricare il nuovo file nel repository.

> Il QR Code deve puntare alla pagina HTML, non direttamente al file vCard.
> In questo modo contatti, link e contenuti possono essere aggiornati senza
> dover ristampare o sostituire il QR Code.

## Pubblicare su GitHub Pages

1. Creare su GitHub un repository chiamato `digital-business-card`.
2. Caricare nella root del repository tutti i file e la cartella `assets`.
3. Aprire **Settings > Pages**.
4. In **Build and deployment**, selezionare **Deploy from a branch**.
5. Selezionare il branch **main** e la cartella **/ (root)**.
6. Salvare e attendere il completamento della pubblicazione.

La pagina sarà disponibile, normalmente entro pochi minuti, all'indirizzo:

```text
https://NOME-UTENTE.github.io/digital-business-card/
```

Se i file si trovano inizialmente dentro la cartella locale
`digital-business-card`, caricare su GitHub il contenuto della cartella, non
una seconda cartella annidata con lo stesso nome.

## Creare un pass Apple Wallet

È possibile usare **Passbook Wallet Pass Creator** o un'applicazione simile.
Configurazione suggerita:

- tipo di pass: **Generic** oppure **Membership**;
- titolo: **Alessandro Esposito**;
- sottotitolo: **Senior Software Engineer & Delivery Manager**;
- QR Code: URL pubblico della landing page GitHub Pages;
- logo e colori: usare il logo FIDES e la palette della pagina.

Anche nel pass Apple Wallet, il QR Code deve puntare alla landing page HTML e
non direttamente alla vCard. La pagina resterà così aggiornabile mantenendo
invariato il pass.

## Aggiornare i dati

Modificare i dati personali sia in `index.html` sia in
`alessandro-esposito.vcf`. Dopo ogni aggiornamento, caricare le modifiche sul
branch `main`; GitHub Pages pubblicherà automaticamente la nuova versione.

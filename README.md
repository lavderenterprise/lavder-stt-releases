<p align="center">
  <img src="assets/hero.svg" alt="Lavder STT, dettatura vocale per macOS" width="100%">
</p>

<p align="center">
  <img alt="macOS 26 o successivo" src="https://img.shields.io/badge/macOS-26%20o%20successivo-0A1018?style=flat-square&logo=apple&logoColor=white">
  <img alt="Apple Silicon" src="https://img.shields.io/badge/chip-Apple%20Silicon-0A1018?style=flat-square">
  <img alt="Notarizzata da Apple" src="https://img.shields.io/badge/notarizzata%20da-Apple-34C759?style=flat-square">
  <img alt="Aggiornamenti automatici" src="https://img.shields.io/badge/aggiornamenti-automatici-F87016?style=flat-square">
  <img alt="Trascrizione on-device" src="https://img.shields.io/badge/trascrizione-on--device-34C759?style=flat-square">
</p>

<p align="center">
  <a href="../../releases/latest">
    <img alt="Scarica l'ultima versione" src="https://img.shields.io/badge/%E2%AC%87%EF%B8%8E%20Scarica%20l'ultima%20versione-F87016?style=for-the-badge&logoColor=white">
  </a>
</p>

<br>

<table>
<tr>
<td width="164" align="center" valign="middle">
  <img src="assets/icon.png" width="132" alt="">
</td>
<td valign="middle">

### Dettatura vocale per macOS, dentro l'app in cui stai lavorando

**Lavder STT** trasforma la voce in testo sul tuo Mac e lo scrive nel campo dove hai il
cursore: la mail aperta, la chat, il terminale, l'editor. Non c'è una finestra intermedia da
cui copiare.

Il motore predefinito è quello di riconoscimento vocale di macOS e lavora senza rete. Whisper
in locale e le API OpenAI restano disponibili come alternative, se ti servono.

</td>
</tr>
</table>

<br>

## Come si detta

Tieni premuta la scorciatoia mentre parli e rilasciala quando hai finito. In alternativa puoi
dettare tenendo premuto il tasto del mouse su un campo di testo, utile quando hai già la mano
sul trackpad.

Mentre parli compare un indicatore vicino alla fotocamera con lo spettro della voce, così sai
che ti sta sentendo. Al rilascio il testo entra nel campo attivo.

<br>

## Cosa la distingue dalla dettatura di sistema

<table>
<tr><td width="56" align="center">📖</td><td><b>Dizionario personale.</b> Nomi propri, sigle aziendali e termini tecnici che il riconoscimento sbaglia sempre allo stesso modo. Aggiungi la parola giusta e la ritrova anche quando la sente storta.</td></tr>
<tr><td width="56" align="center">🧠</td><td><b>Punteggiatura e refusi</b> sistemati dal modello di linguaggio integrato in macOS, senza mandare niente in rete. Richiede Apple Intelligence attiva.</td></tr>
<tr><td width="56" align="center">🔇</td><td><b>Microfono prioritario.</b> Durante la dettatura prende l'esclusiva sul microfono, così chi è in chiamata con te non ti sente. Le app che tengono lo stream sempre aperto, i browser in particolare, restano in ascolto.</td></tr>
<tr><td width="56" align="center">🔉</td><td><b>Audio abbassato</b> mentre detti e riportato al volume di prima quando hai finito.</td></tr>
<tr><td width="56" align="center">📊</td><td><b>Statistiche</b> di parole dettate e tempo risparmiato rispetto alla digitazione.</td></tr>
<tr><td width="56" align="center">⌨️</td><td><b>Modalità appunti</b> per chi preferisce non concedere l'accessibilità: il testo finisce negli appunti e lo incolli con ⌘V.</td></tr>
</table>

<br>

## Installazione

Apri il `.dmg`, trascina **LavderSTT** in **Applicazioni**, avviala da Spotlight.

L'app è firmata con certificato Apple Developer ID e notarizzata da Apple, quindi si apre
senza passare da Impostazioni di Sistema per sbloccarla.

> [!NOTE]
> Non compare nel Dock. Lavder STT sta nella barra dei menu, in alto a destra: cerca l'icona
> del microfono. Se dopo l'avvio sembra non essere successo niente, è lì.

<br>

## I permessi del primo avvio

Una guida introduttiva li chiede uno alla volta. Vanno concessi dall'utente in prima persona:
macOS non consente a nessuna app di autorizzarsi da sola, per quanto firmata.

| Permesso | Serve per | Come arriva |
|---|---|---|
| **Microfono** | registrare quello che detti | richiesta automatica alla prima dettatura |
| **Riconoscimento vocale** | convertire la voce in testo sul Mac | richiesta automatica alla prima dettatura |
| **Accessibilità** | scrivere nel campo dell'app in primo piano | da attivare a mano |

L'accessibilità è l'unico passaggio manuale, perché macOS non permette di richiederla con un
avviso. Si trova in *Impostazioni di Sistema, Privacy e sicurezza, Accessibilità*: cerca
**LavderSTT** nell'elenco e attiva l'interruttore. La guida introduttiva ha un pulsante che
apre direttamente quel pannello.

> [!TIP]
> Se preferisci non concederla, l'app resta utilizzabile: invece di scrivere nel campo attivo
> copia il testo negli appunti.

<br>

## Aggiornamenti

L'app controlla una volta al giorno se è uscita una versione nuova e te la propone. Puoi
forzare il controllo dal menu nella barra o dalle Impostazioni, e disattivarlo da lì se
preferisci decidere tu quando aggiornare.

Non serve tornare su questa pagina a ogni versione.

<br>

## Requisiti

macOS **26** o successivo, su Mac con **Apple Silicon**.

Su versioni precedenti l'app non parte: il riconoscimento vocale e la correzione del testo si
appoggiano a interfacce di sistema introdotte con macOS 26.

<br>

## Privacy

Audio e trascrizione restano sul Mac. Il dizionario personale e il contesto che scrivi nelle
impostazioni sono salvati in locale.

Una sola funzione manda dati fuori, ed è disattivata finché non la accendi tu: il motore di
trascrizione OpenAI, che richiede una tua chiave API e invia l'audio ai server di OpenAI.

<br>

## Come sono firmati gli aggiornamenti

Ogni disk image è firmata con una chiave crittografica di cui l'app conosce soltanto la metà
pubblica. Chi riuscisse a modificare questa pagina o il feed non potrebbe comunque far
installare un programma diverso, perché la firma non tornerebbe e l'app rifiuterebbe il
pacchetto.

<br>

---

<p align="center">
  <sub>
    Qui trovi solo il canale di distribuzione: il feed degli aggiornamenti e le disk image
    firmate. Il codice sorgente è privato.
    <br><br>
    Un progetto <a href="https://github.com/lavderenterprise"><b>Lavder Enterprise</b></a>
  </sub>
</p>

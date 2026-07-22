# Lavder STT

**Dettatura vocale per macOS.** Tieni premuta una scorciatoia, parli, e il testo compare
dove stavi scrivendo — in qualsiasi app.

### [⬇︎ Scarica l'ultima versione](../../releases/latest)

---

## Installazione

1. Apri il file `.dmg` che hai scaricato.
2. Trascina **LavderSTT** dentro la cartella **Applicazioni**.
3. Aprila da Applicazioni (o da Spotlight).

L'app è firmata con un certificato Apple Developer ID e notarizzata da Apple: si apre senza
avvisi di sicurezza e senza dover autorizzare nulla a mano.

> **Non ha icona nel Dock.** Lavder STT vive nella barra dei menu, in alto a destra: cerca
> l'icona del microfono. È normale che aprendola non "succeda niente" a schermo.

## Primo avvio: i permessi

Al primo avvio una breve guida ti chiede tre autorizzazioni. **Deve concederle l'utente di
persona**: macOS non permette a nessuna app, per quanto firmata, di autorizzarsi da sola.

| Permesso | A cosa serve | Quando lo chiede |
|---|---|---|
| **Microfono** | sentire quello che detti | alla prima dettatura, con un avviso |
| **Riconoscimento vocale** | trasformare la voce in testo sul tuo Mac | alla prima dettatura, con un avviso |
| **Accessibilità** | scrivere il testo dettato nell'app in cui stai lavorando | va concesso a mano (vedi sotto) |

**L'accessibilità è l'unico passaggio manuale.** Apri *Impostazioni di Sistema → Privacy e
sicurezza → Accessibilità*, cerca **LavderSTT** nell'elenco e attiva l'interruttore. La guida
introduttiva ha un pulsante che ti porta direttamente su quel pannello.

Senza accessibilità l'app funziona lo stesso, ma invece di inserire il testo te lo copia
negli appunti e devi incollarlo con ⌘V.

## Aggiornamenti

L'app si aggiorna da sola: controlla una volta al giorno e ti propone la nuova versione
quando c'è. Puoi forzare il controllo dal menu nella barra o dalle Impostazioni, e da lì
disattivare il controllo automatico se preferisci.

Non serve tornare su questa pagina né riscaricare il DMG a ogni versione.

## Requisiti

- macOS **26** o successivo
- Mac con **Apple Silicon** (M1 o superiore)

Su versioni precedenti di macOS l'app non si avvia: usa API di riconoscimento vocale e di
intelligenza artificiale che prima non esistevano.

## Privacy

La dettatura funziona **sul tuo Mac**: audio e testo non escono dal computer. Fanno
eccezione due funzioni facoltative, che restano spente finché non le accendi tu: il motore
di trascrizione OpenAI (richiede una tua chiave API) e la traduzione via cloud.

## Sicurezza degli aggiornamenti

Ogni disk image è firmata con una chiave crittografica di cui l'app conosce solo la metà
pubblica. Chi riuscisse a manomettere questa pagina o il feed non potrebbe comunque far
installare un programma diverso: l'app rifiuterebbe la firma.

---

Questo repository contiene **solo** il canale di distribuzione: il feed degli aggiornamenti
e le disk image firmate. Il codice sorgente è privato.

Un progetto **[Lavder Enterprise](https://github.com/lavderenterprise)**.

# Lavder STT — download e aggiornamenti

Canale di distribuzione ufficiale di **Lavder STT**, l'app di dettatura vocale per macOS
di [Lavder Enterprise](https://github.com/lavderenterprise).

## Scarica

Prendi il DMG più recente dalla pagina **[Releases](../../releases/latest)**, aprilo e
trascina *Lavder STT* dentro *Applicazioni*.

L'app è firmata con un certificato Developer ID e notarizzata da Apple: si apre senza
avvisi di Gatekeeper e senza dover autorizzare nulla a mano.

Al primo avvio una breve guida chiede i permessi che servono (microfono, riconoscimento
vocale e accessibilità per inserire il testo dettato dove stai scrivendo).

## Aggiornamenti

Dalla versione 2.4.0 l'app si aggiorna da sola: controlla una volta al giorno e propone
la nuova versione quando c'è. Puoi forzare il controllo dal menu nella barra o dalle
Impostazioni, e disattivare il controllo automatico da lì.

Il file [`appcast.xml`](appcast.xml) è il feed che l'app interroga. Ogni disk image è
firmata con una chiave EdDSA di cui l'app conosce la metà pubblica: un feed manomesso non
basta a far installare un binario estraneo.

## Requisiti

macOS 26 o successivo, Mac con Apple Silicon.

---

Questo repository contiene **solo** il feed degli aggiornamenti e i binari firmati.
Il codice sorgente è privato.

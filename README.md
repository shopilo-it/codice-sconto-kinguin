# Codice sconto Kinguin, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Kinguin** da [shopilo.it](https://shopilo.it/negozi/kinguin.net). Restituisce **coupon Kinguin** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-kinguin](https://shopilo-it.github.io/codice-sconto-kinguin/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-kinguin
cd codice-sconto-kinguin
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Kinguin",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su videogiochi e chiavi digitali",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/kinguin.net"
  }
]
```

## Coupon Kinguin disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su videogiochi e chiavi digitali | [shopilo.it](https://shopilo.it/negozi/kinguin.net) |

Codici attivi: **[shopilo.it/negozi/kinguin.net](https://shopilo.it/negozi/kinguin.net)**

## Domande frequenti

### Come utilizzo un codice sconto Kinguin?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/kinguin.net), aggiungi i prodotti al carrello su Kinguin e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Kinguin?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Kinguin piu recenti?
La pagina [shopilo.it/negozi/kinguin.net](https://shopilo.it/negozi/kinguin.net) viene aggiornata quotidianamente con i codici sconto Kinguin, voucher Kinguin e coupon promozionali Kinguin piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Kinguin

Kinguin e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/kinguin.net) trovi i migliori codici sconto Kinguin, coupon Kinguin verificati e voucher Kinguin attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-kinguin
```

```javascript
const { fetchCoupons } = require('codice-sconto-kinguin');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)

# Codice sconto Vistaprint, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Vistaprint** da [shopilo.it](https://shopilo.it/negozi/vistaprint.it). Restituisce **coupon Vistaprint** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-vistaprint](https://shopilo-it.github.io/codice-sconto-vistaprint/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-vistaprint
cd codice-sconto-vistaprint
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Vistaprint",
    "code": "SHOPILO20",
    "discount": "20%",
    "description": "20% di sconto su stampa personalizzata",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/vistaprint.it"
  }
]
```

## Coupon Vistaprint disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 20% | 20% di sconto su stampa personalizzata | [shopilo.it](https://shopilo.it/negozi/vistaprint.it) |

Codici attivi: **[shopilo.it/negozi/vistaprint.it](https://shopilo.it/negozi/vistaprint.it)**

## Domande frequenti

### Come utilizzo un codice sconto Vistaprint?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/vistaprint.it), aggiungi i prodotti al carrello su Vistaprint e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Vistaprint?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Vistaprint piu recenti?
La pagina [shopilo.it/negozi/vistaprint.it](https://shopilo.it/negozi/vistaprint.it) viene aggiornata quotidianamente con i codici sconto Vistaprint, voucher Vistaprint e coupon promozionali Vistaprint piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Vistaprint

Vistaprint e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/vistaprint.it) trovi i migliori codici sconto Vistaprint, coupon Vistaprint verificati e voucher Vistaprint attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-vistaprint
```

```javascript
const { fetchCoupons } = require('codice-sconto-vistaprint');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)

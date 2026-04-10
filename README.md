# Codice sconto AliExpress, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto AliExpress** da [shopilo.it](https://shopilo.it/negozi/aliexpress.com). Restituisce **coupon AliExpress** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-aliexpress](https://shopilo-it.github.io/codice-sconto-aliexpress/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-aliexpress
cd codice-sconto-aliexpress
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "AliExpress",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% di sconto per nuovi utenti",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/aliexpress.com"
  }
]
```

## Coupon AliExpress disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 15% | 15% di sconto per nuovi utenti | [shopilo.it](https://shopilo.it/negozi/aliexpress.com) |

Codici attivi: **[shopilo.it/negozi/aliexpress.com](https://shopilo.it/negozi/aliexpress.com)**

## Domande frequenti

### Come utilizzo un codice sconto AliExpress?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/aliexpress.com), aggiungi i prodotti al carrello su AliExpress e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon AliExpress?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher AliExpress piu recenti?
La pagina [shopilo.it/negozi/aliexpress.com](https://shopilo.it/negozi/aliexpress.com) viene aggiornata quotidianamente con i codici sconto AliExpress, voucher AliExpress e coupon promozionali AliExpress piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su AliExpress

AliExpress e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/aliexpress.com) trovi i migliori codici sconto AliExpress, coupon AliExpress verificati e voucher AliExpress attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-aliexpress
```

```javascript
const { fetchCoupons } = require('codice-sconto-aliexpress');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)

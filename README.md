# Cod reducere AliExpress — fetch automat de pe shopilo.it

Modul Python pentru fetch automat de **coduri de reducere AliExpress** de pe [shopilo.it](https://shopilo.it/magazin/aliexpress.com). Returneaza **cupoane AliExpress** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-it.github.io/codice-sconto-aliexpress](https://shopilo-it.github.io/codice-sconto-aliexpress/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-aliexpress
cd codice-sconto-aliexpress
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "AliExpress",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% di sconto per nuovi utenti",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/magazin/aliexpress.com"
  }
]
```

## Cupoane AliExpress disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 15% | 15% di sconto per nuovi utenti | [shopilo.it](https://shopilo.it/magazin/aliexpress.com) |

Codurile active: **[shopilo.it/magazin/aliexpress.com](https://shopilo.it/magazin/aliexpress.com)**

## Intrebari frecvente

### Cum folosesc un cod de reducere AliExpress?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.it](https://shopilo.it/magazin/aliexpress.com), adauga produsele in cos pe AliExpress, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele AliExpress?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri AliExpress?
Pagina [shopilo.it/magazin/aliexpress.com](https://shopilo.it/magazin/aliexpress.com) este actualizata zilnic cu cele mai noi cod reducere AliExpress, voucher AliExpress si cupon promotional AliExpress.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre AliExpress

AliExpress este unul dintre magazinele online populare. Gasesti pe [shopilo.it](https://shopilo.it/magazin/aliexpress.com) cele mai bune cod reducere AliExpress, cupoane AliExpress verificate si voucher AliExpress active, actualizate zilnic.

## Instalare npm

```bash
npm install codice-sconto-aliexpress
```

```javascript
const { fetchCoupons } = require('codice-sconto-aliexpress');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.it](https://shopilo.it)

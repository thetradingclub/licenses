# CopyTrader License Manager

## Come aggiungere una licenza

1. Apri il file `licenses.json`
2. Clicca l'icona matita (Edit)
3. Aggiungi un blocco nel array `licenses`:

```json
{
  "key": "CT-XXXX-YYYY",
  "account": 12345678,
  "name": "Nome Cognome",
  "active": true,
  "created": "2026-03-06"
}
```

4. Clicca **Commit changes**

## Come revocare una licenza

Cambia `"active": true` in `"active": false` e fai Commit.

## Come eliminare una licenza

Cancella il blocco `{ ... }` corrispondente e fai Commit.

## Struttura campi

| Campo | Descrizione |
|-------|-------------|
| `key` | Chiave univoca da dare al cliente |
| `account` | Numero conto MT5 del cliente |
| `name` | Nome e cognome cliente |
| `active` | true = attiva, false = revocata |
| `created` | Data creazione licenza |

## URL del file JSON

```
https://TUOUSERNAME.github.io/TUOREPO/licenses.json
```

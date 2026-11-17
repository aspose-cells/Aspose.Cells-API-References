---
title: "Classe PivotCache"
linktitle: "PivotCache"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe PivotCache. Incapsula l'oggetto che rappresenta pivotcache in Go."
type: docs
weight: 200
url: /it/go-cpp/pivotcache/
---

## PivotCache class

Rappresenta la cache di memoria per alcuni report di PivotTable.

```go

type PivotCache struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetMissingItemsLimit](./getmissingitemslimit/) | Ottiene e imposta il numero di elementi inutilizzati da consentire prima di scartare gli elementi inutilizzati. Questo valore DEVE essere maggiore di -2 e minore di 1048577. PivotCacheMissingItemsLimitConst; |
| [SetMissingItemsLimit](./setmissingitemslimit/) | Ottiene e imposta il numero di elementi inutilizzati da consentire prima di scartare gli elementi inutilizzati. Questo valore DEVE essere maggiore di -2 e minore di 1048577. PivotCacheMissingItemsLimitConst; |
| [Refresh_PivotTableRefreshOption](./refresh_pivottablerefreshoption/) | Aggiorna i dati dalla fonte dati e calcola i dati per la visualizzazione di tutte le pivottable la cui fonte dati è questa cache pivot. |
| [Refresh](./refresh/) | Aggiorna i dati dalla fonte dati e calcola i dati per la visualizzazione di tutte le pivottable la cui fonte dati è questa cache pivot. |
| [GetPivotTables](./getpivottables/) | Ottiene tutte le tabelle pivot con questa cache pivot. |
| [Dispose](./dispose/) | Rilascia tutte le risorse. |
| [GetSourceType](./getsourcetype/) | Ottiene il PivotTableSourceType. |

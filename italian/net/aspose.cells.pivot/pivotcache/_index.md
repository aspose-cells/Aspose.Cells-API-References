---
title: "Classe PivotCache"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Pivot.PivotCache. Rappresenta la cache di memoria per alcuni report PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivotcache/
---
## PivotCache class

Rappresenta la cache di memoria per alcuni report PivotTable.

```csharp
public abstract class PivotCache : IDisposable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [MissingItemsLimit](../../aspose.cells.pivot/pivotcache/missingitemslimit/) { get; set; } | Ottiene e imposta il numero di elementi inutilizzati da consentire prima di scartare gli elementi inutilizzati. Questo valore DEVE essere maggiore di -2 e minore di 1048577. [`PivotCacheMissingItemsLimitConst`](../pivotcachemissingitemslimitconst/); |
| abstract [SourceType](../../aspose.cells.pivot/pivotcache/sourcetype/) { get; } | Ottiene il [`PivotTableSourceType`](../pivottablesourcetype/). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| abstract [Dispose](../../aspose.cells.pivot/pivotcache/dispose/)() | Rilascia tutte le risorse. |
| [GetPivotTables](../../aspose.cells.pivot/pivotcache/getpivottables/)() | Ottiene tutte le tabelle pivot con questa cache pivot. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh)() | Aggiorna i dati dalla fonte dati e calcola i dati per la visualizzazione di tutte le tabelle pivot la cui fonte dati è questa cache pivot. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh_1)(PivotTableRefreshOption) | Aggiorna i dati dalla fonte dati e calcola i dati per la visualizzazione di tutte le tabelle pivot la cui fonte dati è questa cache pivot. |

### Osservazioni

Tutti i dati saranno raccolti in questa cache, e la tabella pivot otterrà i dati solo da questa cache, non accedendo direttamente alla fonte dati. Se la fonte dati di alcune [`PivotTable`](../pivottable/) è la stessa, utilizzeranno una cache pivot.

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)



---
title: "PivotCache.Refresh"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotCache. Aggiorna i dati dalla fonte dati e calcola i dati per la visualizzazione di tutte le pivot table la cui fonte dati è questa cache pivot."
type: docs
url: /it/net/aspose.cells.pivot/pivotcache/refresh/
---
## Refresh(PivotTableRefreshOption) {#refresh_1}

Aggiorna i dati dalla fonte dati e calcola i dati per la visualizzazione di tutte le tabelle pivot la cui fonte dati è questa cache pivot.

```csharp
public PivotRefreshState Refresh(PivotTableRefreshOption option)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzione | PivotTableRefreshOption | Le opzioni per aggiornare la fonte dati della pivot table. |

### Osservazioni

È consigliabile chiamare semplicemente [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) per aggiornare tutte le pivot table e i grafici nel file.

### Vedi anche

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Refresh() {#refresh}

Aggiorna i dati dalla fonte dati e calcola i dati per la visualizzazione di tutte le tabelle pivot la cui fonte dati è questa cache pivot.

```csharp
public PivotRefreshState Refresh()
```

### Osservazioni

Se sia table1 che table2 utilizzano questa cache, le due tabelle verranno calcolate. È consigliabile chiamare semplicemente [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) per aggiornare tutte le pivot table e i grafici nel file.

### Vedi anche

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



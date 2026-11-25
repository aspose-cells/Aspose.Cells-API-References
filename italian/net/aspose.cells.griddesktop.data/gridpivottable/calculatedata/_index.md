---
title: "GridPivotTable.CalculateData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridPivotTable. Calcola i dati delle tabelle pivot nelle celle"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridpivottable/calculatedata/
---
## GridPivotTable.CalculateData method

Calcola i dati della pivot table nelle celle.

```csharp
public void CalculateData()
```

### Osservazioni

Cell.Value nell'intervallo pivot potrebbe non restituire il risultato corretto se il metodo non è stato chiamato. Questo metodo calcola i dati con una cache pivot interna, non con la fonte dati originale. Quindi, se la fonte dati viene modificata, si prega di chiamare prima il metodo RefreshData().

### Vedi anche

* class [GridPivotTable](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)



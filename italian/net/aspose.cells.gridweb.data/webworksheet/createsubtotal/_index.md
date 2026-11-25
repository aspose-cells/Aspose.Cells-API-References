---
title: "WebWorksheet.CreateSubtotal"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WebWorksheet. Crea un subtotale nel foglio"
type: docs
url: /it/net/aspose.cells.gridweb.data/webworksheet/createsubtotal/
---
## WebWorksheet.CreateSubtotal method

Crea un subtotale nel foglio.

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList, string functionLabel, 
    GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, NumberType numberType, 
    string customString)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnNameRowIndex | Int32 | L'indice di riga della riga del nome della colonna. |
| dataRows | Int32 | Il numero di righe dati. |
| groupByColumnIndex | Int32 | L'indice della colonna da raggruppare. |
| subtotalFunction | SubtotalFunction | Il tipo di funzione subtotale. |
| subtotalColumnIndexList | Int32[] | Gli indici di colonna da subtotale. |
| functionLabel | String | L'etichetta della funzione subtotale. |
| grandCellStyle | GridTableItemStyle | Lo stile della riga del totale generale. |
| subtotalCellStyle | GridTableItemStyle | Lo stile della riga del subtotale. |
| numberType | NumberType | Il tipo numerico delle celle risultato del subtotale. |
| customString | String | La stringa di formato personalizzato delle celle risultato del subtotale. Può essere null. |

### Vedi anche

* enum [SubtotalFunction](../../subtotalfunction/)
* class [GridTableItemStyle](../../../aspose.cells.gridweb/gridtableitemstyle/)
* enum [NumberType](../../numbertype/)
* class [WebWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)



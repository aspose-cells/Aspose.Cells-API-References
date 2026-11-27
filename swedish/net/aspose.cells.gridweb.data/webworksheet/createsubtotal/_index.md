---
title: "WebWorksheet.CreateSubtotal"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebWorksheet metod. Skapar delsumma i bladet"
type: docs
url: /sv/net/aspose.cells.gridweb.data/webworksheet/createsubtotal/
---
## WebWorksheet.CreateSubtotal method

Skapar delsumma i bladet.

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList, string functionLabel, 
    GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, NumberType numberType, 
    string customString)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnNameRowIndex | Int32 | Radindex för kolumnnamnsraden. |
| dataRows | Int32 | Antalet datarader. |
| groupByColumnIndex | Int32 | Kolumnindex för den kolumn som ska grupperas. |
| subtotalFunction | SubtotalFunction | Typ av subtotalfunktion. |
| subtotalColumnIndexList | Int32[] | Kolumnindex som ska summeras. |
| functionLabel | String | Etiketten för subtotalfunktionen. |
| grandCellStyle | GridTableItemStyle | Stilen för den totala totalsumman. |
| subtotalCellStyle | GridTableItemStyle | Stilen för delsummans rad. |
| numberType | NumberType | Nummertypen för delsummans resultceller. |
| customString | String | Den anpassade formatsträngen för delsummans resultceller. Kan vara null. |

### Se även

* enum [SubtotalFunction](../../subtotalfunction/)
* class [GridTableItemStyle](../../../aspose.cells.gridweb/gridtableitemstyle/)
* enum [NumberType](../../numbertype/)
* class [WebWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)



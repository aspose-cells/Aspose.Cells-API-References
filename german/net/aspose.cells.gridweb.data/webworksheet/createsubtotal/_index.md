---
title: "WebWorksheet.CreateSubtotal"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebWorksheet-Methode. Erstellt eine Zwischensumme im Blatt"
type: docs
url: /de/net/aspose.cells.gridweb.data/webworksheet/createsubtotal/
---
## WebWorksheet.CreateSubtotal method

Erstellt eine Zwischensumme im Blatt.

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList, string functionLabel, 
    GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, NumberType numberType, 
    string customString)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnNameRowIndex | Int32 | Der Zeilenindex der Spaltennamenzeile. |
| dataRows | Int32 | Die Anzahl der Datenzeilen. |
| groupByColumnIndex | Int32 | Der Spaltenindex der zu gruppierenden Spalte. |
| subtotalFunction | SubtotalFunction | Der Typ der Zwischensummenfunktion. |
| subtotalColumnIndexList | Int32[] | Die Spaltenindizes, die zusammengefasst werden sollen. |
| functionLabel | String | Die Bezeichnung der Zwischensummenfunktion. |
| grandCellStyle | GridTableItemStyle | Der Stil der Gesamtsummenzeile. |
| subtotalCellStyle | GridTableItemStyle | Der Stil der Zwischensummenzeile. |
| numberType | NumberType | Der Zahlentyp der Zwischensummen‑Ergebniszellen. |
| customString | String | Der benutzerdefinierte Formatstring der Zwischensummen‑Ergebniszellen. Kann null sein. |

### Siehe auch

* enum [SubtotalFunction](../../subtotalfunction/)
* class [GridTableItemStyle](../../../aspose.cells.gridweb/gridtableitemstyle/)
* enum [NumberType](../../numbertype/)
* class [WebWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)



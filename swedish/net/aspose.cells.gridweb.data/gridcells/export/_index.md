---
title: Export
second_title: Aspose.Cells för .NET API-referens
description: Exporterar data i Cells-samlingen i ett WebWorksheet till ett nytt DataTable-objekt
type: docs
weight: 370
url: /sv/net/aspose.cells.gridweb.data/gridcells/export/
---
## GridCells.Export method

Exporterar data i Cells-samlingen i ett WebWorksheet till ett nytt DataTable-objekt

```csharp
public DataTable Export(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Radnumret för den första cellen som ska exporteras ut. |
| startColumn | Int32 | Kolumnnumret för den första cellen som ska exporteras ut. |
| rows | Int32 | Antal rader som ska importeras. |
| columns | Int32 | Antal kolumner som ska importeras. |
| exportColumnName | Boolean | Anger om data i den första raden exporteras som datatabellens kolumnnamn |
| isVertical | Boolean | Sant om en rad i Excel-fil representerar en rad i DataTable. False om en kolumn i Excel-fil representerar en rad i DataTable. |

### Returvärde

Exporterat DataTable-objekt.

### Se även

* class [GridCells](../../gridcells)
* namnutrymme [Aspose.Cells.GridWeb.Data](../../gridcells)
* hopsättning [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
---
title: "GridCells.Export"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridCells-metod. Exporterar data i Cells-samlingen i ett WebWorksheet till ett nytt DataTable-objekt"
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridcells/export/
---
## GridCells.Export method

Exporterar data i Cells-samlingen för ett WebWorksheet till ett nytt DataTable-objekt

```csharp
public DataTable Export(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Radnumret för den första cellen som ska exporteras. |
| startColumn | Int32 | Kolumnnumret för den första cellen som ska exporteras. |
| rader | Int32 | Antal rader att importera. |
| kolumner | Int32 | Antal kolumner att importera. |
| exportColumnName | Boolean | Anger om data i den första raden exporteras som kolumnnamnet i DataTable |
| ärVertikal | Boolean | Sant om en rad i Excel-filen representerar en rad i DataTable. Falskt om en kolumn i Excel-filen representerar en rad i DataTable. |

### Returvärde

Exporterad DataTable‑objekt.

### Se även

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)



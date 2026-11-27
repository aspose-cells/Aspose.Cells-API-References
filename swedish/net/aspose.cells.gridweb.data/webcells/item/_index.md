---
title: "WebCells.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebCells egenskap. Hämtar Cell-elementet vid angivet cellradindex och kolumnindex"
type: docs
url: /sv/net/aspose.cells.gridweb.data/webcells/item/
---
## WebCells indexer (1 of 2)

Hämtar Cell-elementet vid angivet cellradindex och kolumnindex.

```csharp
public WebCell this[int row, int column] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| row | Radindex. |
| column | Kolumnindex. |

### Returvärde

Cell-objektet.

### Exempel

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells[0, 0];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
Dim cell As Cell =  cells(0,0)  'Gets the cell at "A1"
```

### Se även

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## WebCells indexer (2 of 2)

Hämtar Cell-elementet vid angivet cellnamn.

```csharp
public WebCell this[string cellName] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| cellName | Cellnamn, inklusive dess kolumnbokstav och radnummer, till exempel A5. |

### Returvärde

Ett Cell-objekt

### Exempel

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### Se även

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)



---
title: "WebCells.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebCells Eigenschaft. Gibt das Zellen‑Element am angegebenen Zeilen‑ und Spaltenindex zurück"
type: docs
url: /de/net/aspose.cells.gridweb.data/webcells/item/
---
## WebCells indexer (1 of 2)

Gibt das Zellen‑Element am angegebenen Zeilen‑ und Spaltenindex zurück.

```csharp
public WebCell this[int row, int column] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| row | Zeilenindex. |
| column | Spaltenindex. |

### Rückgabewert

Das Zellenobjekt.

### Beispiele

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells[0, 0];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
Dim cell As Cell =  cells(0,0)  'Gets the cell at "A1"
```

### Siehe auch

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## WebCells indexer (2 of 2)

Gibt das Zellen‑Element mit dem angegebenen Zellenamen zurück.

```csharp
public WebCell this[string cellName] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| cellName | Zellenname, einschließlich seines Spaltenbuchstabens und seiner Zeilennummer, zum Beispiel A5. |

### Rückgabewert

Ein Zellenobjekt

### Beispiele

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### Siehe auch

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)



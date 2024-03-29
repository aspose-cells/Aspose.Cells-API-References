---
title: Cells.Item
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the Cell element at the specified cell row index and column index
type: docs
url: /net/aspose.cells/cells/item/
---
## Cells indexer (1 of 2)

Gets the [`Cell`](../../cell/) element at the specified cell row index and column index.

```csharp
public Cell this[int row, int column] { get; }
```

| Parameter | Description |
| --- | --- |
| row | Row index. |
| column | Column index. |

### Return Value

The [`Cell`](../../cell/) object.

### Examples

```csharp
[C#]
Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells[0, 0];	//Gets the cell at "A1"

[Visual Basic]
Dim excel as Workbook = New Workbook()
Dim cells As Cells =  excel.Worksheets(0).Cells 
Dim cell As Cell =  cells(0,0)  'Gets the cell at "A1"
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Cells indexer (2 of 2)

Gets the [`Cell`](../../cell/) element at the specified cell name.

```csharp
public Cell this[string cellName] { get; }
```

| Parameter | Description |
| --- | --- |
| cellName | Cell name,including its column letter and row number, for example A5. |

### Return Value

A [`Cell`](../../cell/) object

### Examples

```csharp
[C#]
Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]
Dim excel as Workbook = New Workbook()
Dim cells As Cells =  excel.Worksheets(0).Cells 
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



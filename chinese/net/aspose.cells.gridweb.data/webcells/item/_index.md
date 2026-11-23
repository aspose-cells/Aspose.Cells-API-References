---
title: "WebCells.Item"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WebCells 属性。获取指定单元格行索引和列索引处的 Cell 元素"
type: docs
url: /zh/net/aspose.cells.gridweb.data/webcells/item/
---
## WebCells indexer (1 of 2)

获取指定单元格行索引和列索引处的 Cell 元素。

```csharp
public WebCell this[int row, int column] { get; }
```

| 参数 | 描述 |
| --- | --- |
| 行 | 行索引。 |
| 列 | 列索引。 |

### 返回值

Cell 对象。

### 示例

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells[0, 0];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
Dim cell As Cell =  cells(0,0)  'Gets the cell at "A1"
```

### 另请参见

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## WebCells indexer (2 of 2)

获取指定单元格名称处的 Cell 元素。

```csharp
public WebCell this[string cellName] { get; }
```

| 参数 | 描述 |
| --- | --- |
| cellName | 单元格名称，包括其列字母和行号，例如 A5。 |

### 返回值

单元格对象

### 示例

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### 另请参见

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)



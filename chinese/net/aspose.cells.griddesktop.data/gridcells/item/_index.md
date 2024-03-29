---
title: Item
second_title: Aspose.Cells for .NET API 参考
description: 获取Cell工作表中的项目
type: docs
weight: 40
url: /zh/net/aspose.cells.griddesktop.data/gridcells/item/
---
## GridCells indexer (1 of 3)

获取Cell工作表中的项目

```csharp
public GridCell this[int index] { get; }
```

| 范围 | 描述 |
| --- | --- |
| index | 元素的从零开始的索引。 |

### 适当的价值

指定索引处的元素。

### 评论

这是 Cells 类的索引器。 获取指定索引处的单元格元素。

### 也可以看看

* class [GridCell](../../gridcell)
* class [GridCells](../../gridcells)
* 命名空间 [Aspose.Cells.GridDesktop.Data](../../gridcells)
* 部件 [Aspose.Cells.GridDesktop](../../../)

---

## GridCells indexer (2 of 3)

获取Cell指定单元格行索引和列索引处的元素。

```csharp
public GridCell this[int row, int column] { get; }
```

| 范围 | 描述 |
| --- | --- |
| row | 行索引。 |
| column | 列索引。 |

### 返回值

这Cell目的。

### 例子

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells[0, 0];	//获取“A1”处的单元格

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
Dim cell As Cell =  cells(0,0)  'Gets the cell at "A1"
```

### 也可以看看

* class [GridCell](../../gridcell)
* class [GridCells](../../gridcells)
* 命名空间 [Aspose.Cells.GridDesktop.Data](../../gridcells)
* 部件 [Aspose.Cells.GridDesktop](../../../)

---

## GridCells indexer (3 of 3)

获取Cell指定单元格名称处的元素。

```csharp
public GridCell this[string cellName] { get; }
```

| 范围 | 描述 |
| --- | --- |
| cellName | 单元格名称，包括其列字母和行号，例如 A5。 |

### 返回值

一个Cell目的

### 例子

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells["A1"];	//获取“A1”处的单元格

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### 也可以看看

* class [GridCell](../../gridcell)
* class [GridCells](../../gridcells)
* 命名空间 [Aspose.Cells.GridDesktop.Data](../../gridcells)
* 部件 [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->

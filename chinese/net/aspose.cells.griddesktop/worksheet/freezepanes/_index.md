---
title: FreezePanes
second_title: Aspose.Cells for .NET API 参考
description: 在工作表中的指定单元格处冻结窗格
type: docs
weight: 670
url: /zh/net/aspose.cells.griddesktop/worksheet/freezepanes/
---
## FreezePanes(string, int, int) {#freezepanes_1}

在工作表中的指定单元格处冻结窗格。

```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| cellName | String | 单元格名称。 |
| freezedRows | Int32 | 顶部窗格中可见行数，不超过行索引。 |
| freezedColumns | Int32 | 左窗格中可见列的数量，不超过列索引。 |

### 评论

行索引和列索引不能都为零。行数和列数 也不能全部为零。

### 也可以看看

* class [Worksheet](../../worksheet)
* 命名空间 [Aspose.Cells.GridDesktop](../../worksheet)
* 部件 [Aspose.Cells.GridDesktop](../../../)

---

## FreezePanes(int, int, int, int) {#freezepanes}

在工作表中的指定单元格处冻结窗格。

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| row | Int32 | 行索引。 |
| column | Int32 | 列索引。 |
| freezedRows | Int32 | 顶部窗格中可见行数，不超过行索引。 |
| freezedColumns | Int32 | 左窗格中可见列的数量，不超过列索引。 |

### 评论

行索引和列索引不能都为零。行数和列数 也不能全部为零。

前两个参数指定冻结位置，后两个参数指定左上窗格中冻结的区域。

### 也可以看看

* class [Worksheet](../../worksheet)
* 命名空间 [Aspose.Cells.GridDesktop](../../worksheet)
* 部件 [Aspose.Cells.GridDesktop](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->

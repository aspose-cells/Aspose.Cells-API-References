---
title: "WebWorksheet.FreezePanes"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WebWorksheet 方法。冻结工作表中指定单元格处的窗格"
type: docs
url: /zh/net/aspose.cells.gridweb.data/webworksheet/freezepanes/
---
## WebWorksheet.FreezePanes method

在工作表的指定单元格处冻结窗格。

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | Int32 | 行索引。 |
| 列 | Int32 | 列索引。 |
| freezedRows | Int32 | 顶部窗格中可见的行数，不超过行索引。 |
| freezedColumns | Int32 | 左侧窗格中可见的列数，不超过列索引。 |

### 备注

行索引和列索引不能全部为零。行数和列数也不能全部为零。

前两个参数指定冻结位置，后两个参数指定左上窗格中冻结的区域。

### 另请参见

* class [WebWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)



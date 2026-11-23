---
title: "WebCells.Export"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WebCells 方法。将 WebWorksheet 中 Cells 集合的数据导出到一个新的 DataTable 对象"
type: docs
url: /zh/net/aspose.cells.gridweb.data/webcells/export/
---
## WebCells.Export method

将 WebWorksheet 中 Cells 集合的数据导出到新的 DataTable 对象。

```csharp
public DataTable Export(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | Int32 | 要导出的第一个单元格的行号。 |
| startColumn | Int32 | 要导出的第一个单元格的列号。 |
| 行 | Int32 | 要导入的行数。 |
| 列 | Int32 | 要导入的列数。 |
| exportColumnName | 布尔 | 指示第一行的数据是否作为 DataTable 的列名导出 |
| isVertical | 布尔 | 如果 Excel 文件中的行对应 DataTable 中的一行，则为 True；如果 Excel 文件中的列对应 DataTable 中的一行，则为 False。 |

### 返回值

导出的 DataTable 对象。

### 另请参见

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)



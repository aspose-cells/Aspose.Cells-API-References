---
title: "GridJsWorkbook.RedactFile"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "GridJsWorkbook 方法。根据 JSON 操作数组对 Excel 文件执行编辑。"
type: docs
url: /zh/net/aspose.cells.gridjs/gridjsworkbook/redactfile/
---
## GridJsWorkbook.RedactFile method

根据 JSON 操作数组对 Excel 文件执行编辑。

```csharp
public void RedactFile(string excelFilePath, string uid, string[] arrayOfRedactionOpr)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| excelFilePath | String | 待编辑的 Excel 文件的文件路径。 |
| uid | String | 工作簿的唯一标识符。如果为 null 或为空，将根据文件路径生成新的 uid。 |
| arrayOfRedactionOpr | String[] | 表示要应用的编辑操作的 JSON 字符串数组。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [GridCellException](../../gridcellexception/) | 在编辑操作期间出现 CellsException 时抛出。 |
| Exception | 在编辑操作期间出现一般异常时抛出。 |

### 另请参见

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)



---
title: "CellValue.Value"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CellValue 属性。获取或设置单元格值"
type: docs
url: /zh/net/aspose.cells/cellvalue/value/
---
## CellValue.Value property

获取或设置单元格值。

```csharp
public object Value { get; set; }
```

### 备注

值必须是对应于[`Type`](../type/)的正确对象类型：

| **Type** | **Value** |
| --- | --- |
| IsNull | null，任何其他对象将被忽略 |
| IsNumeric | double |
| IsDateTime | DateTime |
| IsString | string |
| IsBool | bool |
| IsError | 错误字符串，例如 "#VALUE!", "#NAME?", ... |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellValuePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CellValue cellValue = new CellValue();
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            worksheet.Cells["A1"].PutValue(cellValue.Value);

            workbook.Save("CellValueDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "类 CellValue"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.CellValue 类。表示单元格值及其对应类型"
type: docs
url: /zh/net/aspose.cells/cellvalue/
---
## CellValue class

表示单元格值及其对应类型。

```csharp
public class CellValue
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [CellValue](cellvalue/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Type](../../aspose.cells/cellvalue/type/) { get; set; } | 获取或设置单元格值的类型。 |
| [Value](../../aspose.cells/cellvalue/value/) { get; set; } | 获取或设置单元格值。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueDemo
    {
        public static void CellValueExample()
        {
            // 创建新工作簿并获取第一个工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建 CellValue 实例
            CellValue cellValue = new CellValue();

            // 设置单元格的类型和值
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            // 将 CellValue 分配给工作表中的单元格
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(cellValue.Value);

            // 保存工作簿
            workbook.Save("CellValueExample.xlsx");
            workbook.Save("CellValueExample.pdf");
            return;
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



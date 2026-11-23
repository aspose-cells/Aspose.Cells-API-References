---
title: "枚举 PivotAreaType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.PivotAreaType 枚举。指示用于描述数据透视表区域或方面的规则类型"
type: docs
url: /zh/net/aspose.cells.pivot/pivotareatype/
---
## PivotAreaType enumeration

指示用于描述数据透视表区域或方面的规则类型。

```csharp
public enum PivotAreaType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `0` | 无数据透视表区域。 |
| Normal | `1` | 表示标题或项目。 |
| Data | `2` | 表示数据区域中的某些内容。 |
| All | `3` | 表示整个数据透视表。 |
| Origin | `4` | 表示数据透视表左上角的空白单元格（对于 RTL 工作表为右上角）。 |
| Button | `5` | 表示字段按钮。 |
| TopRight | `6` | 表示数据透视表右上角的空白单元格（对于 RTL 工作表为左上角）。 |

### 示例

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotAreaTypeDemo
    {
        public static void PivotAreaTypeExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 向工作簿添加新工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apples");
            worksheet.Cells["A3"].PutValue("Oranges");
            worksheet.Cells["A4"].PutValue("Bananas");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);

            // 创建数据透视表
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // 向数据透视表添加字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // 为数据透视表创建 PivotArea
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.OnlyData = true;
            pivotArea.IsRowGrandIncluded = true;

            // 输出 PivotArea 属性
            Console.WriteLine("Pivot Area Type: " + pivotArea.RuleType);
            Console.WriteLine("Only Data: " + pivotArea.OnlyData);
            Console.WriteLine("Is Row Grand Included: " + pivotArea.IsRowGrandIncluded);

            // 保存工作簿
            workbook.Save("PivotAreaTypeExample.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)



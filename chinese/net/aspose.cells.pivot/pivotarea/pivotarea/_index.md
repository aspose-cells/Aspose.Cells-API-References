---
title: "PivotArea.PivotArea"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotArea 构造函数。呈现 PivotTable 的选定区域"
type: docs
url: /zh/net/aspose.cells.pivot/pivotarea/pivotarea/
---
## PivotArea constructor

呈现 PivotTable 的选定区域。

```csharp
public PivotArea(PivotTable table)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 表 | PivotTable |  |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaMethodctorWithPivotTableDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // 向数据透视表添加字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // 演示使用 PivotTable 参数的 PivotArea 构造函数
            PivotArea pivotArea = new PivotArea(pivotTable);
            
            // 配置 PivotArea
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            
            // 保存工作簿
            workbook.Save("PivotAreaDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotTable](../../pivottable/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



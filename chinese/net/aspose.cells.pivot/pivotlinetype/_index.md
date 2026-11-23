---
title: "枚举 PivotLineType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.PivotLineType 枚举。指定 PivotLine 的类型"
type: docs
url: /zh/net/aspose.cells.pivot/pivotlinetype/
---
## PivotLineType enumeration

指定 PivotLine 的类型。

```csharp
public enum PivotLineType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Regular | `0` | 常规 PivotLine，包含透视项。 |
| Subtotal | `1` | 小计行。 |
| GrandTotal | `2` | 总计行。 |
| Blank | `3` | 每个组后都有空行。 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotLineTypeDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // 创建数据透视表
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // 添加行字段和数据字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // 按值对行字段进行降序排序
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "B2");
            
            // 计算数据透视表数据
            pivotTable.CalculateData();
            
            // 保存工作簿
            workbook.Save("PivotLineTypeDemo.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)



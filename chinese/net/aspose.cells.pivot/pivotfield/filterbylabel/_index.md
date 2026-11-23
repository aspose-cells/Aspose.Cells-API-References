---
title: "PivotField.FilterByLabel"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 方法。按行或列透视字段的标题进行筛选"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/filterbylabel/
---
## PivotField.FilterByLabel method

按行或列透视字段的标题进行过滤。

```csharp
public PivotFilter FilterByLabel(PivotFilterType type, string label1, string label2)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 类型 | PivotFilterType | 过滤数据的类型。 |
| label1 | String | 过滤条件的标签 |
| label2 | String | 介于过滤条件的上限标签 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterByLabelWithPivotFilterTypeStringStringDemo
    {
        public static void Run()
        {
            // 创建工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // 添加示例数据
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("");
            sheet.Cells["A5"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["B5"].PutValue(40);

            // 使用正确的参数创建透视表
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // 获取透视字段
            PivotField field = pivot.RowFields[0];
            
            // 应用筛选器
            field.FilterByLabel(PivotFilterType.CaptionNotEqual, "(blank)", "");
            pivot.RefreshData();
            pivot.CalculateData();
            
            // 保存工作簿
            workbook.Save("PivotFilterByLabelDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



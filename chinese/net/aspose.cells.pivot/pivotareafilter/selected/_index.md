---
title: "PivotAreaFilter.Selected"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotAreaFilter 属性。指示此字段是否已选择。仅在 PivotTable 处于大纲视图时有效"
type: docs
url: /zh/net/aspose.cells.pivot/pivotareafilter/selected/
---
## PivotAreaFilter.Selected property

指示此字段是否具有选择。仅在数据透视表处于大纲视图时有效。

```csharp
public bool Selected { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaFilterPropertySelectedDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // 创建数据透视表
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // 获取透视区域过滤器
            PivotArea pivotArea = new PivotArea(pivotTable);
            PivotAreaFilter filter = pivotArea.Filters[0];

            // 显示当前已选择的值
            Console.WriteLine("Current Selected value: " + filter.Selected);

            // 更改已选择的值（仅影响大纲视图）
            filter.Selected = true;
            Console.WriteLine("New Selected value: " + filter.Selected);

            // 保存工作簿
            workbook.Save("PivotAreaFilterSelectedDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



---
title: "PivotFieldSortSetting.IsSimpleSort"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotFieldSortSetting 属性。指示是否将应用简单的数据排序操作"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfieldsortsetting/issimplesort/
---
## PivotFieldSortSetting.IsSimpleSort property

指示是否将应用简单的数据排序操作。

```csharp
public bool IsSimpleSort { get; set; }
```

### 备注

默认值为 true。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyIsSimpleSortDemo
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
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["A6"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;
            worksheet.Cells["B5"].Value = 150;
            worksheet.Cells["B6"].Value = 250;

            // 创建数据透视表
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // 添加行字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // 添加数据字段
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // 获取透视字段
            PivotField pivotField = pivotTable.RowFields[0];

            // 获取排序设置（只读属性）
            PivotFieldSortSetting sortSetting = pivotField.SortSetting;

            // 显示当前 IsSimpleSort 值
            Console.WriteLine("Current IsSimpleSort value: " + sortSetting.IsSimpleSort);

            // 注意：IsSimpleSort 是只读的，因此我们无法直接设置它
            // 为了演示排序，我们将创建一个具有不同排序方式的新数据透视表

            // 创建另一个带有自定义排序的数据透视表
            pivotIndex = pivotTables.Add("A1:B6", "E3", "PivotTable2");
            PivotTable pivotTable2 = pivotTables[pivotIndex];
            pivotTable2.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable2.AddFieldToArea(PivotFieldType.Data, "Sales");

            // 使用可用方法对数据透视字段进行排序
            PivotField pivotField2 = pivotTable2.RowFields[0];
            pivotField2.SortBy(SortOrder.Ascending, -1);

            // 保存工作簿
            workbook.Save("PivotFieldSortSettingPropertyIsSimpleSortDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



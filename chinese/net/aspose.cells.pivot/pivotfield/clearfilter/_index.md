---
title: "PivotField.ClearFilter"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 方法。清除此透视字段的筛选设置"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/clearfilter/
---
## PivotField.ClearFilter method

清除此透视字段的筛选设置。

```csharp
public void ClearFilter()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodClearFilterDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["A4"].Value = "Fruit";
            worksheet.Cells["A5"].Value = "Vegetable";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;
            worksheet.Cells["B5"].Value = 300;

            // 创建数据透视表
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // 添加行字段
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // 添加数据字段
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // 获取透视字段
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // 先应用筛选以演示清除操作
                pivotField.FilterByLabel(PivotFilterType.CaptionEqual, "Fruit", null);

                // 调用 ClearFilter 方法
                pivotField.ClearFilter();

                Console.WriteLine("ClearFilter method executed successfully");
                Console.WriteLine("All filters have been removed from the pivot field");

                // 刷新透视表以显示更改
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFilter method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("PivotFieldMethodClearFilterDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



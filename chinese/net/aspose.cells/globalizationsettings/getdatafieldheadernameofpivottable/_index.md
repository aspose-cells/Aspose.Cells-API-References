---
title: "GlobalizationSettings.GetDataFieldHeaderNameOfPivotTable"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "GlobalizationSettings 方法。获取数据透视表中值区域字段标题的名称"
type: docs
url: /zh/net/aspose.cells/globalizationsettings/getdatafieldheadernameofpivottable/
---
## GlobalizationSettings.GetDataFieldHeaderNameOfPivotTable method

获取数据透视表中值区域字段标题的名称。

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfDataFieldHeader() method instead.")]
public virtual string GetDataFieldHeaderNameOfPivotTable()
```

### 返回值

数据字段标题的名称

### 备注

注意：此成员已过时。请改用 PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() 方法。此属性将在自 2022 年 12 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetDataFieldHeaderNameOfPivotTableDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿并访问第一个工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 200;

            // 设置自定义全局化设置
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // 创建数据透视表并配置字段
                int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B3", "D1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category as row
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);  // Value as data

                // 刷新数据透视表以应用本地化更改
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable created with custom data field header name.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // 保存已修改的工作簿
            workbook.Save("GlobalizationSettingsMethodDemo.xlsx");
        }
    }

    // 自定义 GlobalizationSettings 实现
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetDataFieldHeaderNameOfPivotTable()
        {
            return "Custom Values";
        }
    }
}
```

### 另请参见

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



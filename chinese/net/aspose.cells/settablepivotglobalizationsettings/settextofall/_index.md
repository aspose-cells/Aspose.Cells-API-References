---
title: "SettablePivotGlobalizationSettings.SetTextOfAll"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettablePivotGlobalizationSettings 方法。设置 PivotTable 中 All 标签的文本"
type: docs
url: /zh/net/aspose.cells/settablepivotglobalizationsettings/settextofall/
---
## SettablePivotGlobalizationSettings.SetTextOfAll method

设置 PivotTable 中 "(All)" 标签的文本。

```csharp
public void SetTextOfAll(string text)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文本 | String | 自定义文本 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfAllWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表添加示例数据
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // 创建数据透视表
            var pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // 创建全局化设置
            var settings = new SettableGlobalizationSettings();
            settings.PivotSettings = new SettablePivotGlobalizationSettings();

            try
            {
                // 调用 SetTextOfAll 方法更改 "(All)" 文本
                ((SettablePivotGlobalizationSettings)settings.PivotSettings).SetTextOfAll("All Products");

                // 将设置应用于工作簿
                workbook.Settings.GlobalizationSettings = settings;
                pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium2;

                Console.WriteLine("SetTextOfAll method executed successfully. Changed '(All)' to 'All Products'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextOfAll method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("SettablePivotGlobalizationSettingsMethodSetTextOfAllDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



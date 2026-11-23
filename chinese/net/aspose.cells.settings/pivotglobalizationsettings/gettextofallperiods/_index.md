---
title: "PivotGlobalizationSettings.GetTextOfAllPeriods"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotGlobalizationSettings 方法。获取 All Periods 的本地化文本"
type: docs
url: /zh/net/aspose.cells.settings/pivotglobalizationsettings/gettextofallperiods/
---
## PivotGlobalizationSettings.GetTextOfAllPeriods method

获取 "All Periods" 的本地化文本。

```csharp
public virtual string GetTextOfAllPeriods()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetTextOfAllPeriodsDemo
    {
        public static void Run()
        {
            try
            {
                // 创建一个新的工作簿
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // 添加示例数据以创建透视表的上下文
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["B1"].PutValue("Sales");
                worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
                worksheet.Cells["B2"].PutValue(1000);
                worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
                worksheet.Cells["B3"].PutValue(2000);
                worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
                worksheet.Cells["B4"].PutValue(3000);

                // 创建数据透视表
                int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // 创建 PivotGlobalizationSettings 实例
                PivotGlobalizationSettings settings = new PivotGlobalizationSettings();

                // 演示 GetTextOfAllPeriods 方法
                string allPeriodsText = settings.GetTextOfAllPeriods();
                Console.WriteLine("All Periods Text: " + allPeriodsText);

                // 显示上下文的相关时间段标签
                Console.WriteLine("Years Text: " + settings.GetTextOfYears());
                Console.WriteLine("Quarters Text: " + settings.GetTextOfQuarters());
                Console.WriteLine("Months Text: " + settings.GetTextOfMonths());

                // 保存工作簿
                workbook.Save("GetTextOfAllPeriodsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)



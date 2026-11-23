---
title: "SettableChartGlobalizationSettings.GetLegendIncreaseName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableChartGlobalizationSettings 方法。获取图例中“增加”的名称"
type: docs
url: /zh/net/aspose.cells/settablechartglobalizationsettings/getlegendincreasename/
---
## SettableChartGlobalizationSettings.GetLegendIncreaseName method

获取图例的增加名称。

```csharp
public override string GetLegendIncreaseName()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendIncreaseNameDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加最少的数据以提供上下文
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // 创建 SettableChartGlobalizationSettings 的实例
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // 设置自定义图例增加名称
                settings.SetLegendIncreaseName("Custom Increase Label");

                // 使用 GetLegendIncreaseName 获取图例增加名称
                string legendIncreaseName = settings.GetLegendIncreaseName();
                Console.WriteLine("Legend Increase Name: " + legendIncreaseName);

                // 保存工作簿
                workbook.Save("GetLegendIncreaseNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLegendIncreaseName: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



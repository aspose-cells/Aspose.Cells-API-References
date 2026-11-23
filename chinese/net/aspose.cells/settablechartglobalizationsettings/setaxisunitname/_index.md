---
title: "SettableChartGlobalizationSettings.SetAxisUnitName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableChartGlobalizationSettings 方法。设置轴单位的名称"
type: docs
url: /zh/net/aspose.cells/settablechartglobalizationsettings/setaxisunitname/
---
## SettableChartGlobalizationSettings.SetAxisUnitName method

设置轴单位的名称。

```csharp
public void SetAxisUnitName(DisplayUnitType type, string name)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 类型 | DisplayUnitType | 用于显示坐标轴标签的单位类型。 |
| 名称 | String | 本地依赖名称 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetAxisUnitNameWithDisplayUnitTypeStringDemo
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

                // 为不同的显示单位类型设置自定义坐标轴单位名称
                settings.SetAxisUnitName(DisplayUnitType.Thousands, "K");
                settings.SetAxisUnitName(DisplayUnitType.Millions, "M");
                settings.SetAxisUnitName(DisplayUnitType.Percentage, "Pct");

                // 通过检索值来验证设置
                string thousandsUnit = settings.GetAxisUnitName(DisplayUnitType.Thousands);
                string millionsUnit = settings.GetAxisUnitName(DisplayUnitType.Millions);
                string percentageUnit = settings.GetAxisUnitName(DisplayUnitType.Percentage);

                // 显示结果
                Console.WriteLine($"Thousands unit name set to: {thousandsUnit}");
                Console.WriteLine($"Millions unit name set to: {millionsUnit}");
                Console.WriteLine($"Percentage unit name set to: {percentageUnit}");

                // 保存工作簿
                workbook.Save("SetAxisUnitNameDemo.xlsx");
                Console.WriteLine("SetAxisUnitName method called successfully. Workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetAxisUnitName: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* enum [DisplayUnitType](../../../aspose.cells.charts/displayunittype/)
* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



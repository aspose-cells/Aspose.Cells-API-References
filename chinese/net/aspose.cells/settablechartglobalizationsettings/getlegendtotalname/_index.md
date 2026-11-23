---
title: "SettableChartGlobalizationSettings.GetLegendTotalName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableChartGlobalizationSettings 方法。获取图例的总计名称"
type: docs
url: /zh/net/aspose.cells/settablechartglobalizationsettings/getlegendtotalname/
---
## SettableChartGlobalizationSettings.GetLegendTotalName method

获取图例的总计名称。

```csharp
public override string GetLegendTotalName()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendTotalNameDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些上下文数据
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // 创建 SettableChartGlobalizationSettings 的实例
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // 首先设置自定义图例总计名称
                settings.SetLegendTotalName("Custom Total Label");

                // 调用 GetLegendTotalName 方法以检索该值
                string legendTotalName = settings.GetLegendTotalName();

                // 显示结果
                Console.WriteLine("Legend Total Name: " + legendTotalName);

                // 保存工作簿
                workbook.Save("GetLegendTotalNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLegendTotalName: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



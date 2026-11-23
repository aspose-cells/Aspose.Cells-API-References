---
title: "SettableChartGlobalizationSettings.SetLegendTotalName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableChartGlobalizationSettings 方法。设置图例中“总计”的名称"
type: docs
url: /zh/net/aspose.cells/settablechartglobalizationsettings/setlegendtotalname/
---
## SettableChartGlobalizationSettings.SetLegendTotalName method

设置图例的总计名称。

```csharp
public void SetLegendTotalName(string name)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | String | 本地依赖名称 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetLegendTotalNameWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加最少的数据以提供上下文
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            try
            {
                // 创建 SettableChartGlobalizationSettings 的实例
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // 设置自定义图例总计名称
                settings.SetLegendTotalName("Custom Total Label");

                // 通过获取该值来验证设置
                string legendTotalName = settings.GetLegendTotalName();
                Console.WriteLine("Legend Total Name set to: " + legendTotalName);

                // 保存工作簿
                workbook.Save("SetLegendTotalNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetLegendTotalName: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



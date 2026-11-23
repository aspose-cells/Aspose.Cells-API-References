---
title: "SettableChartGlobalizationSettings.SetChartTitleName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableChartGlobalizationSettings 方法。设置图表标题的名称"
type: docs
url: /zh/net/aspose.cells/settablechartglobalizationsettings/setcharttitlename/
---
## SettableChartGlobalizationSettings.SetChartTitleName method

设置图表标题的名称。

```csharp
public void SetChartTitleName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetChartTitleNameDemo
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

                // 使用自定义字符串调用 SetChartTitleName
                settings.SetChartTitleName("Custom Chart Title");

                // 通过获取该值来验证设置
                string chartTitleName = settings.GetChartTitleName();
                Console.WriteLine("Chart Title Name set to: " + chartTitleName);

                // 保存工作簿
                workbook.Save("SetChartTitleNameDemo.xlsx");
                Console.WriteLine("SetChartTitleName method called successfully. Workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetChartTitleName: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



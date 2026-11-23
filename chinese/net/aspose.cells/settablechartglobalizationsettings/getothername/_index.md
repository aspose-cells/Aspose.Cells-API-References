---
title: "SettableChartGlobalizationSettings.GetOtherName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableChartGlobalizationSettings 方法。获取 Chart 的 Other 标签的名称"
type: docs
url: /zh/net/aspose.cells/settablechartglobalizationsettings/getothername/
---
## SettableChartGlobalizationSettings.GetOtherName method

获取图表的 "Other" 标签名称。

```csharp
public override string GetOtherName()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetOtherNameDemo
    {
        public static void Run()
        {
            // 创建新工作簿并获取第一个工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加最少的数据（可选，仅用于完整的工作簿）
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(250);

            try
            {
                // 实例化全局化设置对象
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // 为 "Other" 标签设置自定义名称
                settings.SetOtherName("Custom Other Label");

                // 使用 GetOtherName 检索名称
                string otherName = settings.GetOtherName();

                Console.WriteLine("Other Name retrieved: " + otherName);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetOtherName: {ex.Message}");
            }

            // 保存工作簿（在此演示中，设置未直接附加到图表）
            workbook.Save("GetOtherNameDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



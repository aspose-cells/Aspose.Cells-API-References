---
title: "SettableGlobalizationSettings.SetLocalFunctionName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。设置与给定标准函数名称对应的区域性依赖函数名称"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/setlocalfunctionname/
---
## SettableGlobalizationSettings.SetLocalFunctionName method

为给定的标准函数名称设置对应的区域性相关函数名称。

```csharp
public void SetLocalFunctionName(string standardName, string localName, bool bidirectional)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| standardName | String | 标准（en-US 区域）函数名。 |
| localName | String | 区域相关的函数名称 |
| bidirectional | Boolean | 是否自动将本地函数名称映射到标准函数名称。如果为 true，则本地名称将自动映射到标准名称，用户无需再次调用 [`SetStandardFunctionName`](../setstandardfunctionname/) 来对应相同的标准和本地名称对 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalFunctionNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建全局化设置
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // 调用 SetLocalFunctionName 将标准函数名称映射为本地名称
                settings.SetLocalFunctionName("SUM", "SOMMA", true); // Italian localization for SUM function
                settings.SetLocalFunctionName("AVERAGE", "MEDIA", true); // Italian localization for AVERAGE function

                // 将设置应用于工作簿
                workbook.Settings.GlobalizationSettings = settings;

                // 使用标准名称和本地化名称创建公式
                worksheet.Cells["A1"].Formula = "=SUM(B1:B5)";
                worksheet.Cells["A2"].Formula = "=SOMMA(B1:B5)";
                worksheet.Cells["A3"].Formula = "=AVERAGE(B1:B5)";
                worksheet.Cells["A4"].Formula = "=MEDIA(B1:B5)";

                // 计算公式
                workbook.CalculateFormula();

                Console.WriteLine("SetLocalFunctionName executed successfully with parameters (String, String, Boolean)");
                Console.WriteLine("Standard and localized function names work equivalently in formulas.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalFunctionName method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("MethodSetLocalFunctionNameWithStringStringBooleanDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



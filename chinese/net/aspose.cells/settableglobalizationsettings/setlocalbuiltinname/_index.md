---
title: "SettableGlobalizationSettings.SetLocalBuiltInName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。设置基于区域设置的文本，用于具有给定标准名称文本的内置名称。"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/setlocalbuiltinname/
---
## SettableGlobalizationSettings.SetLocalBuiltInName method

为给定的标准名称文本设置内置名称的区域性相关文本。

```csharp
public void SetLocalBuiltInName(string standardName, string localName, bool bidirectional)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| standardName | String | 内置名称的标准（en-US 区域）名称文本。 |
| localName | String | 基于区域设置的名称文本 |
| bidirectional | Boolean | 是否自动将本地名称文本映射到标准名称文本。如果为 true，系统会自动将本地名称文本映射到标准名称文本，用户无需再次调用 [`SetStandardBuiltInName`](../setstandardbuiltinname/) 来处理相同的标准和本地名称对。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalBuiltInNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建自定义全局化设置
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // 调用 SetLocalBuiltInName 将标准内置名称映射为本地名称
                settings.SetLocalBuiltInName("SUM", "LOCAL_SUM", true);

                // 将设置应用于工作簿
                workbook.Settings.GlobalizationSettings = settings;

                // 使用标准内置名称创建公式
                worksheet.Cells["A1"].Formula = "=SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 5;
                worksheet.Cells["B2"].Value = 10;
                worksheet.Cells["B3"].Value = 15;

                // 计算公式
                workbook.CalculateFormula();

                Console.WriteLine("Formula with standard built-in name 'SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");

                // 验证本地名称映射
                string localName = settings.GetLocalBuiltInName("SUM");
                Console.WriteLine($"Local name for 'SUM': {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalBuiltInName method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("SetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "SettableGlobalizationSettings.SetStandardFunctionName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。根据给定的标准函数名称设置区域相关的函数名称"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/setstandardfunctionname/
---
## SettableGlobalizationSettings.SetStandardFunctionName method

根据给定的标准函数名称设置区域性相关函数名称。

```csharp
public void SetStandardFunctionName(string localName, string standardName, bool bidirectional)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| localName | String | 区域相关的函数名称 |
| standardName | String | 标准（en-US 区域）函数名。 |
| bidirectional | Boolean | 是否自动将标准函数名称映射到本地函数名称。如果为 true，则标准名称将自动映射到本地名称，用户无需再次调用 [`SetLocalFunctionName`](../setlocalfunctionname/) 来处理相同的标准和本地名称对 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardFunctionNameWithStringStringBooleanDemo
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
                // 调用 SetStandardFunctionName 将本地函数名称映射为标准名称
                settings.SetStandardFunctionName("LOCAL_SUM", "SUM", true);

                // 将设置应用于工作簿
                workbook.Settings.GlobalizationSettings = settings;

                // 使用本地函数名称创建公式
                worksheet.Cells["A1"].Formula = "=LOCAL_SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 10;
                worksheet.Cells["B2"].Value = 20;
                worksheet.Cells["B3"].Value = 30;

                // 计算公式
                workbook.CalculateFormula();

                Console.WriteLine("Formula with local function name 'LOCAL_SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardFunctionName method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("SetStandardFunctionNameDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



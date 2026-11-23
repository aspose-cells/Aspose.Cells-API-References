---
title: "SettableGlobalizationSettings.GetStandardFunctionName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。根据给定的区域相关函数名获取标准函数名"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/getstandardfunctionname/
---
## SettableGlobalizationSettings.GetStandardFunctionName method

根据给定的区域设置相关函数名称获取标准函数名称。

```csharp
public override string GetStandardFunctionName(string localName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| localName | String | 区域相关函数名。该区域由使用此设置的工作簿指定。 |

### 返回值

标准（en-US 区域）函数名。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建自定义全局化设置
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // 设置本地函数名映射
            settings.SetStandardFunctionName("LocalSum", "SUM", true);

            // 将设置应用于工作簿
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // 使用本地函数名调用 GetStandardFunctionName
                string standardName = settings.GetStandardFunctionName("LocalSum");
                
                // 显示结果
                Console.WriteLine($"Standard function name for 'LocalSum' is: {standardName}");

                // 在单元格公式中使用标准函数
                worksheet.Cells["A1"].Formula = $"={standardName}(1,2,3)";
                worksheet.Cells["A2"].Value = 1;
                worksheet.Cells["A3"].Value = 2;
                worksheet.Cells["A4"].Value = 3;

                // 计算公式
                workbook.CalculateFormula();

                // 显示结果
                Console.WriteLine($"Formula result in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }
            
            // 保存工作簿
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



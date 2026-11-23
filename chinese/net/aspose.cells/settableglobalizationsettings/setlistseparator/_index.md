---
title: "SettableGlobalizationSettings.SetListSeparator"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。设置函数列表参数的分隔符 ...等"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/setlistseparator/
---
## SettableGlobalizationSettings.SetListSeparator method

设置列表、函数参数等的分隔符。

```csharp
public void SetListSeparator(char c)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| c | 字符 | 指定的分隔符 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetListSeparatorWithCharDemo
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
                // 使用字符参数调用 SetListSeparator 方法
                settings.SetListSeparator(';');
                
                // 将设置应用于工作簿
                workbook.Settings.GlobalizationSettings = settings;
                
                // 通过创建带列表分隔符的公式来演示其效果
                worksheet.Cells["A1"].Formula = "SUM(1;2;3)";
                worksheet.Cells["A2"].Value = "Formula using custom list separator: SUM(1;2;3)";
                
                Console.WriteLine("SetListSeparator method executed successfully with parameter ';'");
                Console.WriteLine("Formula using custom list separator created in cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetListSeparator method: {ex.Message}");
            }
            
            // 保存结果
            workbook.Save("SetListSeparatorWithCharDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



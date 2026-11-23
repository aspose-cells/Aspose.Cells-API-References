---
title: "SettableGlobalizationSettings.GetStandardBuiltInName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。根据给定的区域相关文本获取内置 Name 的标准文本"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/getstandardbuiltinname/
---
## SettableGlobalizationSettings.GetStandardBuiltInName method

根据给定的区域设置相关文本获取内置名称的标准文本。

```csharp
public override string GetStandardBuiltInName(string localName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| localName | String | 内置 Name 的区域相关文本。该区域由使用此设置的工作簿指定。 |

### 返回值

标准（en-US 区域）文本。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建 SettableGlobalizationSettings 的实例
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            // 设置本地内置名称用于演示
            globalizationSettings.SetLocalBuiltInName("SUM", "LocalSumName", true);

            try
            {
                // 使用本地名称调用 GetStandardBuiltInName 方法
                string standardName = globalizationSettings.GetStandardBuiltInName("LocalSumName");
                
                // 显示结果
                Console.WriteLine($"Standard name for 'LocalSumName' is: {standardName}");

                // 将结果应用到单元格
                worksheet.Cells["A1"].Formula = "=" + standardName + "(1,2,3)";
                workbook.CalculateFormula();

                // 显示计算结果
                Console.WriteLine($"Result of formula in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName method: {ex.Message}");
            }
            
            // 保存工作簿
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "SettableGlobalizationSettings.SetStandardBuiltInName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。根据给定的标准函数名称设置区域相关的函数名称"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/setstandardbuiltinname/
---
## SettableGlobalizationSettings.SetStandardBuiltInName method

根据给定的标准函数名称设置区域性相关函数名称。

```csharp
public void SetStandardBuiltInName(string localName, string standardName, bool bidirectional)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| localName | String | 区域相关的函数名称 |
| standardName | String | 标准（en-US 区域）函数名。 |
| bidirectional | Boolean | 是否自动将标准名称文本映射到本地名称文本。如果为 true，系统会自动将标准名称文本映射到本地名称文本，用户无需再次调用 [`SetLocalBuiltInName`](../setlocalbuiltinname/) 来处理相同的标准和本地名称对。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardBuiltInNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 创建自定义全局化设置
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // 设置工作簿的全局化设置
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // 调用 SetStandardBuiltInName 将本地名称映射为标准内置名称
                // 参数：localName，standardName，bidirectional
                settings.SetStandardBuiltInName("MyLocalName", "SUM", true);
                
                Console.WriteLine("SetStandardBuiltInName executed successfully with parameters (\"MyLocalName\", \"SUM\", true)");
                
                // 通过在公式中使用本地名称来演示效果
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=MyLocalName(A1:A2)";
                
                // 计算公式以展示其在本地名称下的工作效果
                workbook.CalculateFormula();
                Console.WriteLine("Result of formula with local name: " + worksheet.Cells["A3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardBuiltInName method: {ex.Message}");
            }
            
            // 保存结果
            workbook.Save("SetStandardBuiltInNameDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



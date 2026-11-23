---
title: "SettableGlobalizationSettings.GetLocalFunctionName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。根据给定的标准函数名称获取区域设置相关的函数名称"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/getlocalfunctionname/
---
## SettableGlobalizationSettings.GetLocalFunctionName method

根据给定的标准函数名称获取区域设置相关的函数名称。

```csharp
public override string GetLocalFunctionName(string standardName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| standardName | String | 标准（en-US 区域）函数名。 |

### 返回值

区域相关函数名。该区域由使用此设置的工作簿指定。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建自定义全局化设置
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // 为 "SUM" 设置自定义本地函数名称
            settings.SetLocalFunctionName("SUM", "SOMME", true);

            // 将设置应用于工作簿
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // 调用 GetLocalFunctionName 以检索本地化名称
                string localName = settings.GetLocalFunctionName("SUM");
                
                // 显示结果
                Console.WriteLine($"Localized function name for 'SUM': {localName}");

                // 在单元格中使用本地化函数
                worksheet.Cells["A1"].Formula = "=SOMME(B1:B5)";
                worksheet.Cells["B1"].PutValue(1);
                worksheet.Cells["B2"].PutValue(2);
                worksheet.Cells["B3"].PutValue(3);
                worksheet.Cells["B4"].PutValue(4);
                worksheet.Cells["B5"].PutValue(5);

                // 计算公式
                workbook.CalculateFormula();

                // 显示结果
                Console.WriteLine($"Calculation result with localized function: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalFunctionName method: {ex.Message}");
            }
            
            // 保存工作簿
            workbook.Save("MethodGetLocalFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



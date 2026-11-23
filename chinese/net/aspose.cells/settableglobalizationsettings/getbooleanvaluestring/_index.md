---
title: "SettableGlobalizationSettings.GetBooleanValueString"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。获取单元格布尔值的显示字符串"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/getbooleanvaluestring/
---
## SettableGlobalizationSettings.GetBooleanValueString method

获取单元格布尔值的显示字符串。

```csharp
public override string GetBooleanValueString(bool bv)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| bv | 布尔 | 布尔值 |

### 返回值

默认情况下，对 true 值返回 "TRUE"，对 false 值返回 "FALSE"。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetBooleanValueStringWithBooleanDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建自定义全局化设置
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // 设置自定义布尔值字符串
            settings.SetBooleanValueString(true, "TRUE_CUSTOM");
            settings.SetBooleanValueString(false, "FALSE_CUSTOM");

            // 将设置应用于工作簿
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // 使用 true 调用 GetBooleanValueString
                string trueValue = settings.GetBooleanValueString(true);
                Console.WriteLine("Custom true value: " + trueValue);

                // 使用 false 调用 GetBooleanValueString
                string falseValue = settings.GetBooleanValueString(false);
                Console.WriteLine("Custom false value: " + falseValue);

                // 在工作表中演示其效果
                worksheet.Cells["A1"].PutValue(true);
                worksheet.Cells["A2"].PutValue(false);

                Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2 value: " + worksheet.Cells["A2"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBooleanValueString method: {ex.Message}");
            }

            // 保存工作簿
            workbook.Save("SettableGlobalizationSettingsMethodGetBooleanValueStringDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



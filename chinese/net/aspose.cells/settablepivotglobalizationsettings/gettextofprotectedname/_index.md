---
title: "SettablePivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettablePivotGlobalizationSettings 方法。获取指定受保护名称的文本"
type: docs
url: /zh/net/aspose.cells/settablepivotglobalizationsettings/gettextofprotectedname/
---
## SettablePivotGlobalizationSettings.GetTextOfProtectedName method

获取指定受保护名称的文本。

```csharp
public override string GetTextOfProtectedName(string protectedName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| protectedName | String | PivotTable 中的受保护名称。 |

### 返回值

PivotTable 的本地受保护名称。

### 备注

在 Microsoft Excel 中，某些名称不能用作数据透视表中 PivotFields 的名称。这些名称因地区而异，用户可以根据所使用的地区显式指定它们。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfProtectedNameDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些示例数据以供上下文使用
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // 创建 SettablePivotGlobalizationSettings 的实例
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // 为受保护名称设置自定义文本
                settings.SetTextOfProtectedName("Sum", "Total Sum");

                // 获取受保护名称的文本
                string protectedNameText = settings.GetTextOfProtectedName("Sum");

                Console.WriteLine($"Text for protected name 'Sum': {protectedNameText}");

                // 保存工作簿
                workbook.Save("GetTextOfProtectedNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



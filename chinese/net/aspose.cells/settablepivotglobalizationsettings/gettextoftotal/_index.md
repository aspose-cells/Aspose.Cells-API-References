---
title: "SettablePivotGlobalizationSettings.GetTextOfTotal"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettablePivotGlobalizationSettings 方法。获取 PivotTable 中 “Total” 标签的文本。当 PivotTable 在数据区域包含两个或更多 PivotField 时，需要重写此方法"
type: docs
url: /zh/net/aspose.cells/settablepivotglobalizationsettings/gettextoftotal/
---
## SettablePivotGlobalizationSettings.GetTextOfTotal method

获取 PivotTable 中 "Total" 标签的文本。当 PivotTable 在数据区域包含两个或更多 PivotField 时，需要重写此方法。

```csharp
public override string GetTextOfTotal()
```

### 返回值

"Total" 标签的文本

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfTotalDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些示例数据以供上下文使用
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // 创建 SettablePivotGlobalizationSettings 的实例
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // 为 "Total" 标签设置自定义文本
                settings.SetTextOfTotal("Custom Total");

                // 获取 "Total" 标签的文本
                string totalText = settings.GetTextOfTotal();

                Console.WriteLine($"Text of Total: {totalText}");

                // 保存工作簿
                workbook.Save("GetTextOfTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfTotal: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



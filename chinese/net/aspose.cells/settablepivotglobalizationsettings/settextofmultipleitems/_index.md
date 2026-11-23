---
title: "SettablePivotGlobalizationSettings.SetTextOfMultipleItems"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettablePivotGlobalizationSettings 方法。设置数据透视表中 Multiple Items 标签的文本"
type: docs
url: /zh/net/aspose.cells/settablepivotglobalizationsettings/settextofmultipleitems/
---
## SettablePivotGlobalizationSettings.SetTextOfMultipleItems method

设置 PivotTable 中 "(Multiple Items)" 标签的文本。

```csharp
public void SetTextOfMultipleItems(string text)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文本 | String | 自定义文本 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfMultipleItemsWithStringDemo
    {
        public static void Run()
        {
            // 创建新工作簿并获取第一个工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些示例数据（可选，仅用于上下文）
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
                // 为数据透视表中的 "(Multiple Items)" 标签设置自定义文本
                settings.SetTextOfMultipleItems("(Multiple Items Edited)");

                // 检索并显示更新后的文本
                string currentText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Current text of '(Multiple Items)' label: {currentText}");

                // （可选）保存工作簿——此演示不需要数据透视表
                workbook.Save("SetTextOfMultipleItemsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfMultipleItems: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "SettablePivotGlobalizationSettings.SetTextOfColumnLabels"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettablePivotGlobalizationSettings 方法。获取 PivotTable 中列标签的文本"
type: docs
url: /zh/net/aspose.cells/settablepivotglobalizationsettings/settextofcolumnlabels/
---
## SettablePivotGlobalizationSettings.SetTextOfColumnLabels method

获取 PivotTable 中 "Column Labels" 标签的文本。

```csharp
public void SetTextOfColumnLabels(string text)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文本 | String | 列标签的文本 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfColumnLabelsWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿（仅用于上下文）
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // 创建 SettablePivotGlobalizationSettings 的实例
                SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

                // 为 "Column Labels" 标签设置自定义文本
                string customColumnLabel = "My Column Headers";
                settings.SetTextOfColumnLabels(customColumnLabel);

                // 检索当前文本以验证更改
                string currentLabel = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Column Labels text is now: \"{currentLabel}\"");

                // 保存工作簿（此演示不需要数据透视表）
                workbook.Save("SetTextOfColumnLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfColumnLabels: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



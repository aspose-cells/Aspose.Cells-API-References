---
title: "SettablePivotGlobalizationSettings.SetTextOfGrandTotal"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettablePivotGlobalizationSettings 方法。设置数据透视表中 Grand Total 标签的文本"
type: docs
url: /zh/net/aspose.cells/settablepivotglobalizationsettings/settextofgrandtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfGrandTotal method

设置 PivotTable 中 "Grand Total" 标签的文本。

```csharp
public void SetTextOfGrandTotal(string text)
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

    public class SettablePivotGlobalizationSettingsMethodSetTextOfGrandTotalWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新工作簿（仅用于上下文）
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // SettablePivotGlobalizationSettings 的实例
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // 为 "Grand Total" 标签设置自定义文本
                settings.SetTextOfGrandTotal("My Custom Grand Total");

                // 检索更新后的标签文本以验证更改
                string grandTotalText = settings.GetTextOfGrandTotal();

                Console.WriteLine($"Grand Total label text: {grandTotalText}");

                // 保存工作簿，仅用于演示代码能够无错误运行
                workbook.Save("SetTextOfGrandTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfGrandTotal: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



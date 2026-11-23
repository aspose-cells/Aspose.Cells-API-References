---
title: "枚举 HtmlLayoutMode"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Rendering.HtmlLayoutMode 枚举。表示 HTML 渲染的布局模式"
type: docs
url: /zh/net/aspose.cells.rendering/htmllayoutmode/
---
## HtmlLayoutMode enumeration

表示 HTML 渲染的布局模式。

```csharp
public enum HtmlLayoutMode
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Normal | `0` | 渲染类似于 MS Excel 的内容。 |
| Print | `1` | 以打印布局模式渲染内容。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassHtmlLayoutModeDemo
    {
        public static void Run()
        {
            // 创建一个用于演示的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 向工作表添加一些示例数据
                worksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");
                worksheet.Cells["A2"].PutValue("This demonstrates HtmlLayoutMode");

                // 创建 HtmlSaveOptions 并将布局模式设置为 Normal
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                saveOptions.LayoutMode = HtmlLayoutMode.Normal;

                // 使用普通布局模式保存工作簿
                workbook.Save("NormalLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Normal layout mode.");

                // 将布局模式更改为 Print
                saveOptions.LayoutMode = HtmlLayoutMode.Print;

                // 使用打印布局模式保存工作簿
                workbook.Save("PrintLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Print layout mode.");

                // 显示枚举值
                Console.WriteLine($"Normal mode value: {HtmlLayoutMode.Normal}");
                Console.WriteLine($"Print mode value: {HtmlLayoutMode.Print}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HtmlLayoutMode: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)



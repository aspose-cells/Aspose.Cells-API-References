---
title: "HtmlSaveOptions.LayoutMode"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlSaveOptions 属性。获取或设置保存为 HTML 时的布局模式。默认值为 Normal。"
type: docs
url: /zh/net/aspose.cells/htmlsaveoptions/layoutmode/
---
## HtmlSaveOptions.LayoutMode property

获取或设置保存为 HTML 时的布局模式。默认值为 Normal。

```csharp
public HtmlLayoutMode LayoutMode { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyLayoutModeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些示例数据
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Layout Mode Test");

            try
            {
                // 创建 HtmlSaveOptions 实例
                HtmlSaveOptions options = new HtmlSaveOptions();

                // 显示当前 LayoutMode 值。
                Console.WriteLine("Current LayoutMode: " + options.LayoutMode);

                // 将 LayoutMode 设置为 Print。
                options.LayoutMode = HtmlLayoutMode.Print;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // 使用 Print 布局模式保存工作簿。
                workbook.Save("LayoutModePrint.html", options);

                // 将 LayoutMode 设置为 Normal。
                options.LayoutMode = HtmlLayoutMode.Normal;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // 使用 Normal 布局模式保存工作簿。
                workbook.Save("LayoutModeNormal.html", options);

                Console.WriteLine("HTML files saved with different LayoutMode settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* enum [HtmlLayoutMode](../../../aspose.cells.rendering/htmllayoutmode/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



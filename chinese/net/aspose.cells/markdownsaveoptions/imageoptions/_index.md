---
title: "MarkdownSaveOptions.ImageOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "MarkdownSaveOptions 属性。在导出之前获取 ImageOrPrintOptions 对象。"
type: docs
url: /zh/net/aspose.cells/markdownsaveoptions/imageoptions/
---
## MarkdownSaveOptions.ImageOptions property

在导出之前获取 ImageOrPrintOptions 对象。

```csharp
public ImageOrPrintOptions ImageOptions { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class MarkdownSaveOptionsPropertyImageOptionsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 创建示例工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些数据以使示例更有意义
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "Image Options Demo";

            try
            {
                // 创建 MarkdownSaveOptions 实例
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // 访问 ImageOptions 属性（只读）。
                ImageOrPrintOptions imageOptions = saveOptions.ImageOptions;

                // 显示 ImageOptions 属性的当前值。
                Console.WriteLine("ImageOptions properties:");
                Console.WriteLine($"HorizontalResolution: {imageOptions.HorizontalResolution}");
                Console.WriteLine($"VerticalResolution: {imageOptions.VerticalResolution}");
                Console.WriteLine($"ImageType: {imageOptions.ImageType}");
                Console.WriteLine($"Quality: {imageOptions.Quality}");
                Console.WriteLine($"Transparent: {imageOptions.Transparent}");

                // 使用当前选项保存工作簿。
                workbook.Save("ImageOptionsDemo.md", saveOptions);

                Console.WriteLine("Markdown file saved successfully with ImageOptions demonstrated.");
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

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



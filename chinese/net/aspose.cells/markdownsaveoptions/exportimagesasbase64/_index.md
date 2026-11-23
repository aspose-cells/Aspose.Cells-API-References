---
title: "MarkdownSaveOptions.ExportImagesAsBase64"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "MarkdownSaveOptions 属性。指定是否将图像以 Base64 格式保存到 Markdown。默认值为 true"
type: docs
url: /zh/net/aspose.cells/markdownsaveoptions/exportimagesasbase64/
---
## MarkdownSaveOptions.ExportImagesAsBase64 property

指定是否将图像以 Base64 格式保存到 Markdown。默认值为 true。

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### 备注

当此属性设置为 true 时，图像数据直接导出到 img 元素中，不会创建单独的文件。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据和图像
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("With Image");

            // 向工作表添加图像
            int imageIndex = worksheet.Pictures.Add(1, 1, "sample.png");

            try
            {
                // 创建 MarkdownSaveOptions 实例
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // 显示 ExportImagesAsBase64 的默认值
                Console.WriteLine("Default ExportImagesAsBase64 value: " + saveOptions.ExportImagesAsBase64);

                // 将 ExportImagesAsBase64 设置为 false 以演示该属性
                saveOptions.ExportImagesAsBase64 = false;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // 使用 ExportImagesAsBase64 = false 保存
                workbook.Save("MarkdownImagesAsFiles.md", saveOptions);

                // 将 ExportImagesAsBase64 设置为 true
                saveOptions.ExportImagesAsBase64 = true;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // 使用 ExportImagesAsBase64 = true 保存
                workbook.Save("MarkdownImagesAsBase64.md", saveOptions);

                Console.WriteLine("Markdown files saved with different ExportImagesAsBase64 settings.");
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

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



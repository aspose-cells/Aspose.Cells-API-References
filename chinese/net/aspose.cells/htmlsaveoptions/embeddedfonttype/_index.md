---
title: "HtmlSaveOptions.EmbeddedFontType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlSaveOptions 属性。获取或设置嵌入字体文件到 html 文件的类型。默认值为 None，表示不会在 html 中嵌入任何字体。"
type: docs
url: /zh/net/aspose.cells/htmlsaveoptions/embeddedfonttype/
---
## HtmlSaveOptions.EmbeddedFontType property

获取或设置嵌入字体文件到 html 文件的类型。默认值为 None，表示不会在 html 中嵌入任何字体。

```csharp
public HtmlEmbeddedFontType EmbeddedFontType { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些示例数据
            worksheet.Cells["A1"].PutValue("Sample Text with Font");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);

            try
            {
                // 创建 HTML 保存选项
                HtmlSaveOptions options = new HtmlSaveOptions();

                // 显示默认的 EmbeddedFontType 值。
                Console.WriteLine("Default EmbeddedFontType: " + options.EmbeddedFontType);

                // 将 EmbeddedFontType 设置为 Woff。
                options.EmbeddedFontType = HtmlEmbeddedFontType.Woff;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // 以 WOFF 字体嵌入方式保存工作簿。
                workbook.Save("EmbeddedFontType_Woff.html", options);

                // 重置为 None。
                options.EmbeddedFontType = HtmlEmbeddedFontType.None;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // 在不嵌入字体的情况下保存工作簿。
                workbook.Save("EmbeddedFontType_None.html", options);

                Console.WriteLine("EmbeddedFontType demonstration completed successfully.");
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

* enum [HtmlEmbeddedFontType](../../../aspose.cells.rendering/htmlembeddedfonttype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "MarkdownSaveOptions.AlignColumnPadding"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "MarkdownSaveOptions 属性。指示是否为生成的 Markdown 表格启用列对齐。启用时，列通过使用指定字符（通常为空格）填充单元格内容来对齐。将其设置为 0 可禁用列对齐（默认）。"
type: docs
url: /zh/net/aspose.cells/markdownsaveoptions/aligncolumnpadding/
---
## MarkdownSaveOptions.AlignColumnPadding property

指示是否为生成的 Markdown 表格启用列对齐。启用时，列通过使用指定字符（通常为 ' ' 空格）填充单元格内容来对齐。将其设置为 '\\0' 可禁用列对齐（默认）。

```csharp
public char AlignColumnPadding { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyAlignColumnPaddingDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据以演示列对齐。
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "1.99";
            worksheet.Cells["C2"].Value = "10";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = "0.99";
            worksheet.Cells["C3"].Value = "20";

            // 创建 MarkdownSaveOptions 实例
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // 显示默认的 AlignColumnPadding 值。
                Console.WriteLine("Default AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // 将 AlignColumnPadding 设置为空格字符以实现列对齐。
                saveOptions.AlignColumnPadding = ' ';

                // 显示更新后的值
                Console.WriteLine("Updated AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // 将工作簿保存为带列对齐的 markdown。
                workbook.Save("AlignColumnPaddingDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with column alignment enabled.");
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



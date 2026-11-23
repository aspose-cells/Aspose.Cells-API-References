---
title: "HtmlSaveOptions.DisableCss"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlSaveOptions 属性。指示是否仅在不依赖 CSS 的情况下应用内联样式。默认值为 false"
type: docs
url: /zh/net/aspose.cells/htmlsaveoptions/disablecss/
---
## HtmlSaveOptions.DisableCss property

指示是否仅在不依赖 CSS 的情况下应用内联样式。默认值为 false。

```csharp
public bool DisableCss { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyDisableCssDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据和格式
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;
            worksheet.Cells["B1"].PutValue("Formatted Cell");
            worksheet.Cells["B1"].GetStyle().Font.IsItalic = true;
            worksheet.Cells["B1"].GetStyle().Font.Underline = FontUnderlineType.Single;

            // 创建 HtmlSaveOptions 实例
            HtmlSaveOptions options = new HtmlSaveOptions();

            // 显示当前 DisableCss 值
            Console.WriteLine("Current DisableCss value: " + options.DisableCss);

            // 将 DisableCss 设置为 true（使用内联样式而非 CSS）
            options.DisableCss = true;
            workbook.Save("HtmlWithInlineStyles.html", options);

            // 将 DisableCss 设置为 false（使用 CSS 样式）
            options.DisableCss = false;
            workbook.Save("HtmlWithCssStyles.html", options);

            // 比较输出文件以查看样式方法的差异
            Console.WriteLine("Files saved with different DisableCss settings.");
        }
    }
}
```

### 另请参见

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



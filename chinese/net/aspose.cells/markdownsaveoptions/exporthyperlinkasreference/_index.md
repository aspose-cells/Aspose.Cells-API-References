---
title: "MarkdownSaveOptions.ExportHyperlinkAsReference"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "MarkdownSaveOptions 属性。指示是否使用引用定义而非内联格式导出超链接。默认值为 false"
type: docs
url: /zh/net/aspose.cells/markdownsaveoptions/exporthyperlinkasreference/
---
## MarkdownSaveOptions.ExportHyperlinkAsReference property

指示是否使用引用定义而非内联格式导出超链接。默认值为 false。

```csharp
public bool ExportHyperlinkAsReference { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportHyperlinkAsReferenceDemo
    {
        public static void Run()
        {
            // 创建新工作簿并获取第一个工作表
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // 在单元格中放入示例文本
            sheet.Cells["A1"].PutValue("Visit Aspose");

            // 向单元格 (A1) 添加超链接
            // 参数：firstRow, firstColumn, totalRows, totalColumns, hyperlink
            sheet.Hyperlinks.Add(0, 0, 1, 1, "https://www.aspose.com");

            // 初始化 Markdown 保存选项
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // 直接访问 ExportHyperlinkAsReference 属性（此演示中为只读）
                Console.WriteLine("ExportHyperlinkAsReference value: " + saveOptions.ExportHyperlinkAsReference);

                // 将工作簿保存为 markdown；如果属性为 true，将影响超链接的导出方式
                workbook.Save("ExportHyperlinkAsReferenceDemo.md", saveOptions);
                Console.WriteLine("Workbook saved as markdown.");
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



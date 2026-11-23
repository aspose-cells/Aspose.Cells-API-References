---
title: "HtmlSaveOptions.ExportCommentsType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlSaveOptions 属性。表示导出注释到 HTML 文件的类型"
type: docs
url: /zh/net/aspose.cells/htmlsaveoptions/exportcommentstype/
---
## HtmlSaveOptions.ExportCommentsType property

表示导出注释到 HTML 文件的类型。

```csharp
public PrintCommentsType ExportCommentsType { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportCommentsTypeDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 使用单元格名称添加示例注释
            Comment comment = worksheet.Comments["A1"];
            comment.Note = "This is a test comment";
            
            // 使用 ExportCommentsType 设置 HTML 保存选项。
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportCommentsType = PrintCommentsType.PrintInPlace;
            
            // 保存为 HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file with comments exported successfully.");
        }
    }
}
```

### 另请参见

* enum [PrintCommentsType](../../printcommentstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



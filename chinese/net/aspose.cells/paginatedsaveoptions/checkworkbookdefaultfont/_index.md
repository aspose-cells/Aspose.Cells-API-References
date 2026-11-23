---
title: "PaginatedSaveOptions.CheckWorkbookDefaultFont"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PaginatedSaveOptions 属性。当 Excel 中的字符为 Unicode 且单元格样式未设置正确字体时，它们可能在 pdfimage 中显示为方块。将此属性设为 true，尝试使用工作簿的默认字体首先显示这些字符"
type: docs
url: /zh/net/aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/
---
## PaginatedSaveOptions.CheckWorkbookDefaultFont property

当 Excel 中的字符是 Unicode 且单元格样式未设置正确的字体时，它们可能在 PDF、图像中显示为方块。将此设置为 true 可尝试首先使用工作簿的默认字体来显示这些字符。

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### 备注

默认值为 true。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyCheckWorkbookDefaultFontDemo
    {
        public static void Run()
        {
            // 创建示例工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Test Content");
            
            // 配置 PDF 保存选项
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.CheckWorkbookDefaultFont = false;
            
            // 保存为 PDF
            workbook.Save("output.pdf", saveOptions);
            
            Console.WriteLine("PDF saved with CheckWorkbookDefaultFont set to false");
        }
    }
}
```

### 另请参见

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



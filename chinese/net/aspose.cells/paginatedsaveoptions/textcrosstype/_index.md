---
title: "PaginatedSaveOptions.TextCrossType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PaginatedSaveOptions 属性。获取或设置当文本宽度大于单元格宽度时的显示文本类型"
type: docs
url: /zh/net/aspose.cells/paginatedsaveoptions/textcrosstype/
---
## PaginatedSaveOptions.TextCrossType property

获取或设置当文本宽度大于单元格宽度时的显示文本类型。

```csharp
public TextCrossType TextCrossType { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyTextCrossTypeDemo
    {
        public static void Run()
        {
            // 创建包含示例数据的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 设置会跨越单元格边界的长文本
            worksheet.Cells["A1"].PutValue("This is a long text that will cross cell boundaries");
            worksheet.Cells["B1"].PutValue("Another cell content");
            
            // 设置列宽以使文本跨单元格
            worksheet.Cells.SetColumnWidth(0, 5);
            
            // 创建 PDF 保存选项
            PdfSaveOptions options = new PdfSaveOptions();
            
            // 通过将 TextCrossType 设置为 CrossKeep 来演示
            options.TextCrossType = TextCrossType.CrossKeep;
            
            // 将工作簿另存为 PDF
            workbook.Save("TextCrossTypeDemo.pdf", options);
            
            Console.WriteLine("PDF saved with TextCrossType.CrossKeep setting");
        }
    }
}
```

### 另请参见

* enum [TextCrossType](../../textcrosstype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



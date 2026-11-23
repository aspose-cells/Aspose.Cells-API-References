---
title: "PaginatedSaveOptions.PageIndex"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PaginatedSaveOptions 属性。获取或设置要保存的第一页的 0 基索引"
type: docs
url: /zh/net/aspose.cells/paginatedsaveoptions/pageindex/
---
## PaginatedSaveOptions.PageIndex property

获取或设置要保存的第一页的零基索引。

```csharp
public int PageIndex { get; set; }
```

### 备注

默认值为 0。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // 创建包含示例数据的新工作簿
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // 在多个页面上添加示例数据
            for (int i = 0; i < 100; i++)
            {
                sheet.Cells[i, 0].Value = "Data " + (i + 1);
            }

            // 设置 PDF 保存选项
            PdfSaveOptions options = new PdfSaveOptions();
            
            // 设置为打印第 3-4 页（基于 0 的索引）
            options.PageIndex = 2;  // Third page (index 2)
            options.PageCount = 2; // Print 2 pages
            
            // 使用选定的页面保存 PDF
            wb.Save("SelectedPages.pdf", options);
            
            Console.WriteLine("PDF with pages 3-4 created successfully.");
        }
    }
}
```

### 另请参见

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



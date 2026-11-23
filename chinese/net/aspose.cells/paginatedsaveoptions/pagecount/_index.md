---
title: "PaginatedSaveOptions.PageCount"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PaginatedSaveOptions 属性。获取或设置要保存的页数"
type: docs
url: /zh/net/aspose.cells/paginatedsaveoptions/pagecount/
---
## PaginatedSaveOptions.PageCount property

获取或设置要保存的页数。

```csharp
public int PageCount { get; set; }
```

### 备注

默认值为 System.Int32.MaxValue，表示将渲染所有页面。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageCountDemo
    {
        public static void Run()
        {
            // 打开 Excel 文件
            Workbook wb = new Workbook("Book1.xlsx");
            
            // 初始化 PDF 保存选项
            PdfSaveOptions options = new PdfSaveOptions();
            
            // 设置仅打印从第 4 页开始的 2 页（基于 0 的索引为 3）
            options.PageIndex = 3;
            options.PageCount = 2;
            
            // 保存 PDF 文件
            wb.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with selected pages.");
        }
    }
}
```

### 另请参见

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



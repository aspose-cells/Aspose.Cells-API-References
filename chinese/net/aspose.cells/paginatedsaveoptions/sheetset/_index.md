---
title: "PaginatedSaveOptions.SheetSet"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PaginatedSaveOptions 属性。获取或设置要渲染的工作表。默认是工作簿中所有可见的工作表（Visible）"
type: docs
url: /zh/net/aspose.cells/paginatedsaveoptions/sheetset/
---
## PaginatedSaveOptions.SheetSet property

获取或设置要呈现的工作表。默认是工作簿中所有可见的工作表：[`Visible`](../../../aspose.cells.rendering/sheetset/visible/)。

```csharp
public SheetSet SheetSet { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // 创建一个包含两个工作表的新工作簿
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // 在两个工作表中设置一些示例数据
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // 创建 PDF 保存选项
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // 使用 SheetSet 仅保存第二个工作表
            pdfSaveOptions.SheetSet = new SheetSet(new int[] { 1 }); // 0-based index
            
            // 使用指定的工作表保存工作簿
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### 另请参见

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



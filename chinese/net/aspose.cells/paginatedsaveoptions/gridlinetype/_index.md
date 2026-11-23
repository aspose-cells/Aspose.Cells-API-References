---
title: "PaginatedSaveOptions.GridlineType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PaginatedSaveOptions 属性。获取或设置网格线类型"
type: docs
url: /zh/net/aspose.cells/paginatedsaveoptions/gridlinetype/
---
## PaginatedSaveOptions.GridlineType property

获取或设置网格线类型。

```csharp
public GridlineType GridlineType { get; set; }
```

### 备注

默认值为 Dotted 类型。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyGridlineTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加示例数据并启用网格线
            worksheet.Cells["A1"].PutValue("GridlineType Demo");
            worksheet.Cells["B2"].PutValue(1);
            worksheet.Cells["C3"].PutValue(2);
            worksheet.Cells["D4"].PutValue(3);
            worksheet.IsGridlinesVisible = true;

            // 创建 PDF 保存选项
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // 演示 GridlineType 属性
            pdfSaveOptions.GridlineType = GridlineType.Dotted;

            // 保存带有网格线的工作簿
            workbook.Save("GridlineTypeDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### 另请参见

* enum [GridlineType](../../gridlinetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



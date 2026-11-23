---
title: "PptxSaveOptions.ExportViewType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PptxSaveOptions 属性。获取和设置导出到 PowerPoint 时的显示类型。默认的导出类型是以打印方式工作"
type: docs
url: /zh/net/aspose.cells/pptxsaveoptions/exportviewtype/
---
## PptxSaveOptions.ExportViewType property

获取和设置导出到 PowerPoint 时的显示类型。默认的导出类型是以打印方式工作。

```csharp
public SlideViewType ExportViewType { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyExportViewTypeDemo
    {
        public static void Run()
        {
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // 使用 ExportViewType 设置 PPTX 保存选项
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.ExportViewType = SlideViewType.View;
            
            // 将工作簿保存为 PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("Workbook saved as PPTX with ExportViewType set to View");
        }
    }
}
```

### 另请参见

* enum [SlideViewType](../../../aspose.cells.slides/slideviewtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



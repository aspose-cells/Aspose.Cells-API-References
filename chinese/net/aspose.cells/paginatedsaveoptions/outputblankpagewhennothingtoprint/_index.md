---
title: "PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PaginatedSaveOptions 属性。指示在没有内容可打印时是否输出空白页"
type: docs
url: /zh/net/aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/
---
## PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint property

指示在没有内容可打印时是否输出空白页。

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### 备注

默认值为 true。

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 添加一个工作表并将其隐藏（模拟没有可打印内容）
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.IsVisible = false;

            // 将 PDF 保存选项的 OutputBlankPageWhenNothingToPrint 设置为 false
            PdfSaveOptions options = new PdfSaveOptions
            {
                OutputBlankPageWhenNothingToPrint = false
            };

            // 保存为 PDF - 不应生成空白页
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputNoBlankPage.pdf");
            workbook.Save(outputPath, options);

            // 将该选项改为 true
            options.OutputBlankPageWhenNothingToPrint = true;

            // 再次保存 - 应生成空白页
            outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputWithBlankPage.pdf");
            workbook.Save(outputPath, options);
        }
    }
}
```

### 另请参见

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



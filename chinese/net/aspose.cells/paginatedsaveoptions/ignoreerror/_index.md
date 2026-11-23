---
title: "PaginatedSaveOptions.IgnoreError"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PaginatedSaveOptions 属性。指示在渲染时是否需要隐藏错误。错误可能出现在形状、图像、图表渲染等方面"
type: docs
url: /zh/net/aspose.cells/paginatedsaveoptions/ignoreerror/
---
## PaginatedSaveOptions.IgnoreError property

指示在渲染时是否需要隐藏错误。错误可能出现在形状、图像、图表渲染等方面。

```csharp
public bool IgnoreError { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // 创建包含示例数据的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加一些可能包含格式错误的示例数据
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);
            
            // 创建 PDF 保存选项
            PdfSaveOptions options = new PdfSaveOptions();
            
            // 将 IgnoreError 设置为 true，以跳过任何转换错误
            options.IgnoreError = true;
            
            // 将工作簿另存为 PDF
            workbook.Save("PaginatedSaveWithIgnoreError.pdf", options);
            
            Console.WriteLine("PDF saved with IgnoreError enabled.");
        }
    }
}
```

### 另请参见

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "PaginatedSaveOptions.OnePagePerSheet"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PaginatedSaveOptions 属性。如果 OnePagePerSheet 为 true，单个工作表的所有内容将仅输出到结果中的一页。pagesetup 的纸张大小将无效，而 pagesetup 的其他设置仍然生效"
type: docs
url: /zh/net/aspose.cells/paginatedsaveoptions/onepagepersheet/
---
## PaginatedSaveOptions.OnePagePerSheet property

如果 OnePagePerSheet 为 true，单个工作表的所有内容将仅输出为结果中的一页。pagesetup 的纸张尺寸将失效，其他 pagesetup 设置仍然生效。

```csharp
public bool OnePagePerSheet { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyOnePagePerSheetDemo
    {
        public static void Run()
        {
            // 创建一个带有测试数据的示例工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            
            // 向两个工作表添加一些示例数据
            for (int i = 0; i < 10; i++)
            {
                sheet1.Cells[i, 0].Value = $"Sheet1 Data {i + 1}";
                sheet2.Cells[i, 0].Value = $"Sheet2 Data {i + 1}";
            }

            // 使用 OnePagePerSheet 设置 PDF 保存选项
            PdfSaveOptions options = new PdfSaveOptions();
            options.OnePagePerSheet = true;

            // 将工作簿保存为 PDF
            workbook.Save("output.pdf", options);
        }
    }
}
```

### 另请参见

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



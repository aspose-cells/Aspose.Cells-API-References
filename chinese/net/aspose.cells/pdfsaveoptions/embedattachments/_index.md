---
title: "PdfSaveOptions.EmbedAttachments"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PdfSaveOptions 属性。指示是否为 Excel 中的 Ole 对象嵌入附件"
type: docs
url: /zh/net/aspose.cells/pdfsaveoptions/embedattachments/
---
## PdfSaveOptions.EmbedAttachments property

指示是否为 Excel 中的 Ole 对象嵌入附件。

```csharp
public bool EmbedAttachments { get; set; }
```

### 备注

默认值为 false。当设置 PDF/A 合规或启用 PDF 加密时，该值必须为 false。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;
using System.IO;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyEmbedAttachmentsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF with Embedded Attachments Example");

            // 创建用于嵌入的示例文件
            string sampleFile = "sample.docx";
            File.WriteAllText(sampleFile, "This is a sample document");

            // 向工作表添加附件（OLE 对象）
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(sampleFile));
            worksheet.OleObjects[oleIndex].FileFormatType = FileFormatType.Docx;
            worksheet.OleObjects[oleIndex].DisplayAsIcon = true;

            // 创建 PDF 保存选项
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // 将 EmbedAttachments 属性设置为 true
            pdfSaveOptions.EmbedAttachments = true;

            // 将工作簿另存为带嵌入附件的 PDF
            workbook.Save("PdfWithEmbeddedAttachments.pdf", pdfSaveOptions);

            // 清理
            File.Delete(sampleFile);
        }
    }
}
```

### 另请参见

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



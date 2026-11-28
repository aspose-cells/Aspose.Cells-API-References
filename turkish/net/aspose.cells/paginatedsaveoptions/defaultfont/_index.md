---
title: "PaginatedSaveOptions.DefaultFont"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaginatedSaveOptions özelliği. Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa pdfimage'de blok olarak görünebilirler. Bu karakterleri göstermek için MingLiu veya MS Gothic gibi DefaultFont'u ayarlayın. Bu özellik ayarlanmamışsa Aspose.Cells bu Unicode karakterleri göstermek için sistemin varsayılan yazı tipini kullanacaktır"
type: docs
url: /tr/net/aspose.cells/paginatedsaveoptions/defaultfont/
---
## PaginatedSaveOptions.DefaultFont property

Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf ve görüntüde blok olarak görünebilirler. Bu karakterleri göstermek için MingLiu veya MS Gothic gibi bir DefaultFont ayarlayın. Bu özellik ayarlanmamışsa, Aspose.Cells bu Unicode karakterleri göstermek için sistemin varsayılan yazı tipini kullanacaktır.

```csharp
public string DefaultFont { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyDefaultFontDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("This text will use the default font");
            worksheet.Cells["A2"].PutValue("如果默认字体支持中文，这将显示正确");

            // Varsayılan yazı tipiyle PDF kaydetme seçeneklerini yapılandırın
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.DefaultFont = "宋体";
            pdfSaveOptions.CheckWorkbookDefaultFont = true;

            // PDF'ye kaydet
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



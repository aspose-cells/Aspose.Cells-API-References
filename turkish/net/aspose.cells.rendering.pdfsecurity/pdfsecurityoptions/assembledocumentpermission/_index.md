---
title: "PdfSecurityOptions.AssembleDocumentPermission"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSecurityOptions özelliği. ModifyDocumentPermission açık olsa bile, belgeyi birleştirmeye, sayfa eklemeye, döndürmeye veya silmeye ve yer imleri ya da küçük resim oluşturmasına izin verilip verilmediğini gösterir."
type: docs
url: /tr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/assembledocumentpermission/
---
## PdfSecurityOptions.AssembleDocumentPermission property

Belgenin birleştirilmesine (sayfa ekleme, döndürme veya silme ve yer imleri ya da küçük resim oluşturma) izin verilip verilmediğini gösterir, hatta [`ModifyDocumentPermission`](../modifydocumentpermission/) açık olsa bile.

```csharp
public bool AssembleDocumentPermission { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyAssembleDocumentPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            pdfSecurityOptions.OwnerPassword = "owner123";
            pdfSecurityOptions.UserPassword = "user123";
            pdfSecurityOptions.AssembleDocumentPermission = false;
            pdfSecurityOptions.PrintPermission = true;

            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
            workbook.Save("secured_document.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with assemble document permission disabled.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)



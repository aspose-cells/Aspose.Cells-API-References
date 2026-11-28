---
title: "PdfSecurityOptions.ExtractContentPermissionObsolete"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSecurityOptions özelliği. PDF referansına göre içerik kopyalama veya çıkarma izni artık kullanılmamaktadır"
type: docs
url: /tr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermissionobsolete/
---
## PdfSecurityOptions.ExtractContentPermissionObsolete property

İçerik kopyalama veya çıkarma izni PDF referansına göre artık kullanılmamaktadır.

```csharp
[Obsolete("Use ExtractContentPermission property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ExtractContentPermissionObsolete { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ExtractContentPermission özelliğini kullanın. Bu özellik Eylül 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyExtractContentPermissionObsoleteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            pdfSecurityOptions.OwnerPassword = "owner123";
            pdfSecurityOptions.UserPassword = "user123";
            pdfSecurityOptions.ExtractContentPermissionObsolete = false;
            pdfSecurityOptions.ExtractContentPermission = true;

            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
            workbook.Save("SecurePDF.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ExtractContentPermissionObsolete set to false");
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)



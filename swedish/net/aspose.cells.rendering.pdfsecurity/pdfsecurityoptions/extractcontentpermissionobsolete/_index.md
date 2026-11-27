---
title: "PdfSecurityOptions.ExtractContentPermissionObsolete"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSecurityOptions-egenskap. Tillstånd att kopiera eller extrahera innehåll som föråldrats enligt PDF-referensen"
type: docs
url: /sv/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermissionobsolete/
---
## PdfSecurityOptions.ExtractContentPermissionObsolete property

Tillstånd att kopiera eller extrahera innehåll som föråldrats enligt PDF-referensen.

```csharp
[Obsolete("Use ExtractContentPermission property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ExtractContentPermissionObsolete { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället ExtractContentPermission-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med september 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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

### Se även

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)



---
title: "PdfSecurityOptions.FullQualityPrintPermission"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSecurityOptions-Eigenschaft. Gibt an, ob das Drucken des Dokuments zu einer Darstellung erlaubt ist, aus der eine getreue digitale Kopie des PDF-Inhalts erzeugt werden kann."
type: docs
url: /de/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fullqualityprintpermission/
---
## PdfSecurityOptions.FullQualityPrintPermission property

Gibt an, ob das Drucken des Dokuments zu einer Darstellung, aus der eine getreue digitale Kopie des PDF‑Inhalts erzeugt werden kann, erlaubt ist.

```csharp
public bool FullQualityPrintPermission { get; set; }
```

### Hinweise

Wenn sie nicht gesetzt ist (und [`PrintPermission`](../printpermission/) gesetzt ist), ist der Druck auf eine niedrigstufige Darstellung des Erscheinungsbildes beschränkt, möglicherweise von verminderter Qualität.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyFullQualityPrintPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test Full Quality Print Permission";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.FullQualityPrintPermission = true;
            securityOptions.PrintPermission = true;

            saveOptions.SecurityOptions = securityOptions;
            workbook.Save("FullQualityPrintDemo.pdf", saveOptions);

            Console.WriteLine("PDF created with FullQualityPrintPermission enabled.");
        }
    }
}
```

### Siehe auch

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)



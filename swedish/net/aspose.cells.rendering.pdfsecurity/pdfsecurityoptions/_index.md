---
title: "Klass PdfSecurityOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.PdfSecurity.PdfSecurityOptions-klass. Alternativ för kryptering och åtkomstbehörigheter för ett PDF-dokument. PDF/A tillåter inte säkerhetsinställningar"
type: docs
url: /sv/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/
---
## PdfSecurityOptions class

Alternativ för kryptering och åtkomstbehörigheter för ett PDF-dokument. PDF/A tillåter inte säkerhetsinställningar.

```csharp
public class PdfSecurityOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PdfSecurityOptions](pdfsecurityoptions/)() | Konstruktorn för PdfSecurityOptions |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AccessibilityExtractContent](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/accessibilityextractcontent/) { get; set; } | Anger om det ska tillåtas att extrahera text och grafik (för att stödja tillgänglighet för användare med funktionsnedsättningar eller för andra ändamål). |
| [AnnotationsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/annotationspermission/) { get; set; } | Anger om det ska tillåtas att lägga till eller ändra textanteckningar, fylla i interaktiva formulärfält. |
| [AssembleDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/assembledocumentpermission/) { get; set; } | Anger om det ska tillåtas att sammanställa dokumentet (infoga, rotera eller ta bort sidor samt skapa bokmärken eller miniatyrbilder), även om [`ModifyDocumentPermission`](./modifydocumentpermission/) är tydlig. |
| [ExtractContentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermission/) { get; set; } | Anger om det ska tillåtas att kopiera eller på annat sätt extrahera text och grafik från dokumentet genom operationer som inte styrs av [`AccessibilityExtractContent`](./accessibilityextractcontent/). |
| [ExtractContentPermissionObsolete](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermissionobsolete/) { get; set; } | (**Obsolete.**) Tillstånd att kopiera eller extrahera innehåll föråldrat enligt PDF-referensen. |
| [FillFormsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fillformspermission/) { get; set; } | Indikerar om det ska tillåtas att fylla i befintliga interaktiva formulärfält (inklusive signaturfält), även om [`ModifyDocumentPermission`](./modifydocumentpermission/) är klar. |
| [FullQualityPrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fullqualityprintpermission/) { get; set; } | Indikerar om det ska tillåtas att skriva ut dokumentet till en representation från vilken en trogen digital kopia av PDF-innehållet kan genereras. |
| [ModifyDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/) { get; set; } | Indikerar om det ska tillåtas att ändra dokumentets innehåll genom operationer som inte kontrolleras av [`AnnotationsPermission`](./annotationspermission/), [`FillFormsPermission`](./fillformspermission/) och [`AssembleDocumentPermission`](./assembledocumentpermission/). |
| [OwnerPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/) { get; set; } | Hämtar eller anger ägarlösenordet för det krypterade PDF-dokumentet. |
| [PrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/printpermission/) { get; set; } | Indikerar om det ska tillåtas att skriva ut dokumentet. |
| [UserPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/) { get; set; } | Hämtar eller anger användarlösenordet som krävs för att öppna det krypterade PDF-dokumentet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Rendering.PdfSecurity;
    using System;

    public class PdfSecurityOptionsDemo
    {
        public static void PdfSecurityOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Aspose";

            // Skapa PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Skapa PdfSecurityOptions
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            // Ställ in säkerhetsalternativ
            pdfSecurityOptions.OwnerPassword = "YourOwnerPassword";
            pdfSecurityOptions.UserPassword = "YourUserPassword";
            pdfSecurityOptions.PrintPermission = true;
            pdfSecurityOptions.ModifyDocumentPermission = false;
            pdfSecurityOptions.ExtractContentPermissionObsolete = false;
            pdfSecurityOptions.AnnotationsPermission = true;
            pdfSecurityOptions.FillFormsPermission = true;
            pdfSecurityOptions.ExtractContentPermission = false;
            pdfSecurityOptions.AccessibilityExtractContent = true;
            pdfSecurityOptions.AssembleDocumentPermission = false;
            pdfSecurityOptions.FullQualityPrintPermission = true;

            // Tilldela säkerhetsalternativ till PdfSaveOptions
            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

            // Save the workbook as a PDF with the specified security options
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering.PdfSecurity](../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../)



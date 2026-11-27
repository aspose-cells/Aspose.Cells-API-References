---
title: "PaginatedSaveOptions.CheckFontCompatibility"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions-egenskap. Anger om teckensnittskompatibilitet ska kontrolleras för varje tecken i texten"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/checkfontcompatibility/
---
## PaginatedSaveOptions.CheckFontCompatibility property

Anger om teckensnittskompatibilitet ska kontrolleras för varje tecken i texten.

```csharp
public bool CheckFontCompatibility { get; set; }
```

### Anmärkningar

Standardvärdet är true. Att inaktivera denna egenskap kan ge bättre prestanda. Men när standard- eller angivet teckensnitt för text/tecken inte kan användas för att rendera det, kan oläsliga tecken (t.ex. block) uppstå i den genererade pdf-filen. I sådana situationer bör användaren behålla denna egenskap som true så att ett alternativt teckensnitt kan sökas och användas för att rendera texten istället;

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyCheckFontCompatibilityDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Compatibility Test");

            // Skapa paginerade sparalternativ
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Demonstrera CheckFontCompatibility-egenskapen
            saveOptions.CheckFontCompatibility = false; // Disable font compatibility checking
            
            // Ställ in andra nödvändiga egenskaper
            saveOptions.DefaultFont = "Arial";
            saveOptions.CheckWorkbookDefaultFont = true;

            // Spara dokumentet med de angivna alternativen
            workbook.Save("PaginatedSaveOptions_CheckFontCompatibility.pdf", saveOptions);
            
            Console.WriteLine("Document saved with CheckFontCompatibility = false");
        }
    }
}
```

### Se även

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



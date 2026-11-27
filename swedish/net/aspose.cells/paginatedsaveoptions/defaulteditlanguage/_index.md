---
title: "PaginatedSaveOptions.DefaultEditLanguage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions egenskap. Hämtar eller anger standardredigeringsspråk"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/defaulteditlanguage/
---
## PaginatedSaveOptions.DefaultEditLanguage property

Hämtar eller anger standardspråket för redigering.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Anmärkningar

Den kan visa/rendera olika layouter för textparagraf när olika redigeringsspråk är inställda. Standard är Auto.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite CJK-text för att demonstrera DefaultEditLanguage-egenskapen
            worksheet.Cells["A1"].PutValue("日本語のテキスト");
            worksheet.Cells["A2"].PutValue("中文文本");
            worksheet.Cells["A3"].PutValue("한글 텍스트");

            // Skapa PDF-sparalternativ och ange CJK som standardredigeringsspråk
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;
            
            // Spara arbetsboken med de angivna alternativen
            workbook.Save("output.pdf", pdfSaveOptions);
            
            Console.WriteLine("Workbook saved with CJK as default edit language.");
        }
    }
}
```

### Se även

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



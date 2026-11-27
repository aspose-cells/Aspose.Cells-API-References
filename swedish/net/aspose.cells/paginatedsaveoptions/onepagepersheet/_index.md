---
title: "PaginatedSaveOptions.OnePagePerSheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions egenskap. Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig och de andra inställningarna i pagesetup kommer fortfarande att gälla"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/onepagepersheet/
---
## PaginatedSaveOptions.OnePagePerSheet property

Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig, men de övriga inställningarna i pagesetup kommer fortfarande att gälla.

```csharp
public bool OnePagePerSheet { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok med testdata
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            
            // Lägg till lite exempeldata i båda bladen
            for (int i = 0; i < 10; i++)
            {
                sheet1.Cells[i, 0].Value = $"Sheet1 Data {i + 1}";
                sheet2.Cells[i, 0].Value = $"Sheet2 Data {i + 1}";
            }

            // Ställ in PDF-sparalternativ med OnePagePerSheet
            PdfSaveOptions options = new PdfSaveOptions();
            options.OnePagePerSheet = true;

            // Spara arbetsboken som PDF
            workbook.Save("output.pdf", options);
        }
    }
}
```

### Se även

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



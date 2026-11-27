---
title: "PaginatedSaveOptions.AllColumnsInOnePagePerSheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions-egenskap. Om AllColumnsInOnePagePerSheet är true kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. Bredden på pappersstorleken i pagesetup kommer att ignoreras och de andra inställningarna i pagesetup kommer fortfarande att gälla"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/
---
## PaginatedSaveOptions.AllColumnsInOnePagePerSheet property

Om AllColumnsInOnePagePerSheet är true, kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. Bredden på pappersstorleken i sidinställningarna kommer att ignoreras, och de andra inställningarna för sidinställningarna kommer fortfarande att tillämpas.

```csharp
public bool AllColumnsInOnePagePerSheet { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyAllColumnsInOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att demonstrera kolumnanpassning
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[0, i].PutValue("Column " + (i + 1));
                worksheet.Cells[1, i].PutValue("Sample data " + (i + 1));
            }

            // Skapa PDF-sparalternativ
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.OnePagePerSheet = true;
            pdfSaveOptions.AllColumnsInOnePagePerSheet = true;

            // Spara arbetsboken med alternativen
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with all columns in one page per sheet.");
        }
    }
}
```

### Se även

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "LowCodeSaveOptions.SaveFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptions-egenskap. Hämtar och anger sparformatet för utdata. Generellt för specifika processer i lågkodssätt är endast vissa specifika format tillåtna. Ange det korrekta formatet för motsvarande process, annars kan oväntade resultat eller till och med undantag uppstå."
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptions/saveformat/
---
## LowCodeSaveOptions.SaveFormat property

Hämtar och anger sparaformatet för utdata. Generellt, för specifika processer på lågkodssätt, är endast vissa specifika format tillåtna. Ange det korrekta formatet för motsvarande process, annars kan oväntade resultat eller till och med undantag uppstå.

```csharp
public virtual SaveFormat SaveFormat { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);

            // Initiera LowCodeSaveOptions med olika format
            LowCodeSaveOptions excelOptions = new LowCodeSaveOptions();
            LowCodeSaveOptions pdfOptions = new LowCodeSaveOptions();

            // Konfigurera Excel-sparalternativ
            excelOptions.SaveFormat = SaveFormat.Xlsx;
            excelOptions.OutputFile = "output_excel.xlsx";

            // Konfigurera PDF‑sparalternativ
            pdfOptions.SaveFormat = SaveFormat.Pdf;
            pdfOptions.OutputFile = "output_pdf.pdf";

            // Demonstrera sparande i originalformat
            Console.WriteLine($"Saving as {excelOptions.SaveFormat}");
            workbook.Save(excelOptions.OutputFile, excelOptions.SaveFormat);

            // Demonstrera formatändring och spara igen
            Console.WriteLine($"Changing format to {pdfOptions.SaveFormat}");
            Console.WriteLine($"Saving as {pdfOptions.SaveFormat}");
            workbook.Save(pdfOptions.OutputFile, pdfOptions.SaveFormat);

            Console.WriteLine("Files saved successfully with different formats.");
        }
    }
}
```

### Se även

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)



---
title: "Klass LowCodePdfSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.LowCodePdfSaveOptions-klass. Alternativ för att spara PDF på lågkodsätt"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodepdfsaveoptions/
---
## LowCodePdfSaveOptions class

Alternativ för att spara PDF på ett lågt kodsätt.

```csharp
public class LowCodePdfSaveOptions : LowCodeSaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [LowCodePdfSaveOptions](lowcodepdfsaveoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Hämtar och anger filen (med sökväg om behövs) för att spara den genererade datan. När denna egenskap sätts till ett värde annat än null eller tom sträng, kommer [`OutputStream`](../lowcodesaveoptions/outputstream/) att ignoreras. (Arv från [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Hämtar och anger strömmen för att skriva den genererade datan till. När den här egenskapen sätts till ett värde annat än null, kommer [`OutputFile`](../lowcodesaveoptions/outputfile/) att ignoreras. (Ärvd från [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [PdfOptions](../../aspose.cells.lowcode/lowcodepdfsaveoptions/pdfoptions/) { get; set; } | Alternativen för att spara PDF-fil. |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodepdfsaveoptions/saveformat/) { get; set; } | Sparaformatet för utdata. För konvertering till PDF kan det endast vara PDF. |

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodePdfSaveOptionsDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Skapa PDF-sparalternativ
            PdfSaveOptions pdfOptions = new PdfSaveOptions();
            pdfOptions.Compliance = PdfCompliance.PdfA1b;

            // Skapa lågkod PDF-sparalternativ
            LowCodePdfSaveOptions lowCodePdfOptions = new LowCodePdfSaveOptions()
            {
                OutputFile = "output.pdf",
                PdfOptions = pdfOptions
            };

            // Spara med lågkodsalternativ
            workbook.Save(lowCodePdfOptions.OutputFile, lowCodePdfOptions.PdfOptions);

            Console.WriteLine("File saved successfully with LowCodePdfSaveOptions");
        }
    }
}
```

### Se även

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)



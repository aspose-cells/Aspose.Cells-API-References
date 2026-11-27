---
title: "Klass LowCodeHtmlSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.LowCodeHtmlSaveOptions-klass. Alternativ för att spara html på lågkodssätt"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/
---
## LowCodeHtmlSaveOptions class

Alternativ för att spara HTML på ett lågt kodsätt.

```csharp
public class LowCodeHtmlSaveOptions : LowCodeSaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [LowCodeHtmlSaveOptions](lowcodehtmlsaveoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [HtmlOptions](../../aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/) { get; set; } | De allmänna alternativen för att spara html. |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Hämtar och anger filen (med sökväg om behövs) för att spara den genererade datan. När denna egenskap sätts till ett värde annat än null eller tom sträng, kommer [`OutputStream`](../lowcodesaveoptions/outputstream/) att ignoreras. (Arv från [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Hämtar och anger strömmen för att skriva den genererade datan till. När den här egenskapen sätts till ett värde annat än null, kommer [`OutputFile`](../lowcodesaveoptions/outputfile/) att ignoreras. (Ärvd från [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodehtmlsaveoptions/saveformat/) { get; set; } | Hämtar och anger formatet för kalkylbladet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeHtmlSaveOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Widget");
            worksheet.Cells["B2"].PutValue(29.99);

            // Skapa och konfigurera LowCodeHtmlSaveOptions
            LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
            {
                HtmlOptions = new HtmlSaveOptions()
                {
                    ExportWorksheetCSSSeparately = false,
                    ExportImagesAsBase64 = true
                }
            };

            // Spara arbetsbok med konfigurerade HTML-alternativ med hjälp av sparalternativparametern
            workbook.Save("LowCodeHtmlExport.html", saveOptions.HtmlOptions);

            Console.WriteLine("HTML file saved successfully with low code options.");
        }
    }
}
```

### Se även

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)



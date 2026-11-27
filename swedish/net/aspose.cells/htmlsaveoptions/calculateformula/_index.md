---
title: "HtmlSaveOptions.CalculateFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Anger om formler ska beräknas innan HTML-filen sparas"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/calculateformula/
---
## HtmlSaveOptions.CalculateFormula property

Anger om formler ska beräknas innan html‑filen sparas.

```csharp
public bool CalculateFormula { get; set; }
```

### Anmärkningar

Standardvärdet är falskt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data och formler i kalkylbladet
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Skapa HtmlSaveOptions med CalculateFormula satt till sant
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                CalculateFormula = true
            };

            // Spara arbetsboken som HTML – formler kommer att beräknas
            workbook.Save("HtmlWithCalculatedFormulas.html", saveOptions);

            Console.WriteLine("HTML file with calculated formulas created successfully.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



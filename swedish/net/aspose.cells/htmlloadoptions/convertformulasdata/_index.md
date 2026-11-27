---
title: "HtmlLoadOptions.ConvertFormulasData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlLoadOptions-egenskap. Om true konverteras strängen till formel när strängvärdet börjar med tecknet, standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/htmlloadoptions/convertformulasdata/
---
## HtmlLoadOptions.ConvertFormulasData property

Om true, konvertera strängen till formel när strängvärdet börjar med tecknet '=', standardvärdet är false.

```csharp
[Obsolete("Use HtmlLoadOptions.HasFormula property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ConvertFormulasData { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället HtmlLoadOptions.HasFormula‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med mars 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyConvertFormulasDataDemo
    {
        public static void Run()
        {
            // Skapa en instans av HtmlLoadOptions
            HtmlLoadOptions options = new HtmlLoadOptions();

            // Ställ in ConvertFormulasData‑egenskapen till true
            options.ConvertFormulasData = true;

            // Läs in en HTML-fil i en arbetsbok med de angivna alternativen
            Workbook workbook = new Workbook("input.html", options);

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Visa några cellvärden för att demonstrera formelkonvertering
            Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell B1 formula: " + worksheet.Cells["B1"].Formula);

            // Spara arbetsboken till en Excel-fil
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



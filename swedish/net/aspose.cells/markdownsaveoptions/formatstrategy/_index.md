---
title: "MarkdownSaveOptions.FormatStrategy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MarkdownSaveOptions‑egenskap. Hämtar och anger formatstrategin när cellvärdet exporteras som sträng"
type: docs
url: /sv/net/aspose.cells/markdownsaveoptions/formatstrategy/
---
## MarkdownSaveOptions.FormatStrategy property

Hämtar och anger formatstrategin när cellvärdet exporteras som sträng.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med olika format
            worksheet.Cells["A1"].PutValue(123.456); // Numeric value
            worksheet.Cells["A2"].PutValue(DateTime.Now); // Date value
            worksheet.Cells["A3"].PutValue(true); // Boolean value

            // Skapa Markdown‑sparalternativ med DisplayString‑formatstrategi
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                FormatStrategy = CellValueFormatStrategy.DisplayString
            };

            // Spara arbetsboken som Markdown
            workbook.Save("MarkdownWithDisplayString.md", saveOptions);

            // Byt till CellValueFormatStrategy.CellStyle
            saveOptions.FormatStrategy = CellValueFormatStrategy.CellStyle;
            workbook.Save("MarkdownWithCellStyle.md", saveOptions);

            Console.WriteLine("Markdown files saved successfully with different format strategies.");
        }
    }
}
```

### Se även

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



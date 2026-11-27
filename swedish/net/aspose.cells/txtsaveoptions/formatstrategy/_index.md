---
title: "TxtSaveOptions.FormatStrategy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtSaveOptions-egenskap. Hämtar och anger formatstrategin när cellvärdet exporteras som sträng"
type: docs
url: /sv/net/aspose.cells/txtsaveoptions/formatstrategy/
---
## TxtSaveOptions.FormatStrategy property

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
    public class TxtSaveOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange värden med olika format
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(599.99);

            // Applicera talformat på priser
            Style style = workbook.CreateStyle();
            style.Number = 2; // Format as currency
            worksheet.Cells["B2:B3"].SetStyle(style);

            // Konfigurera textsparalternativ med olika formatstrategier
            TxtSaveOptions options = new TxtSaveOptions
            {
                Separator = '\t',
                FormatStrategy = CellValueFormatStrategy.DisplayStyle // Show formatted values
            };

            // Spara med visningsformatering
            workbook.Save("FormattedOutput.txt", options);

            // Ändra till ingen formateringsstrategi
            options.FormatStrategy = CellValueFormatStrategy.None;
            workbook.Save("RawOutput.txt", options);

            Console.WriteLine("Files saved with different format strategies.");
        }
    }
}
```

### Se även

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



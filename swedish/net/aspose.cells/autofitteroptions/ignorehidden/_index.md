---
title: "AutoFitterOptions.IgnoreHidden"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFitterOptions-egenskap. Ignorerar dolda rader/kolumner"
type: docs
url: /sv/net/aspose.cells/autofitteroptions/ignorehidden/
---
## AutoFitterOptions.IgnoreHidden property

Ignorerar dolda rader/kolumner.

```csharp
public bool IgnoreHidden { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyIgnoreHiddenDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in exempeldata och formatera rader
            worksheet.Cells["A1"].PutValue("This is a test string for autofit");
            worksheet.Cells["A2"].PutValue("Another test string");
            
            // Dölj rad 1
            worksheet.Cells.Rows[1].IsHidden = true;

            // Skapa AutoFitterOptions med IgnoreHidden satt till true
            AutoFitterOptions options = new AutoFitterOptions
            {
                IgnoreHidden = true,
                AutoFitMergedCells = false,
                OnlyAuto = false
            };

            // Autoanpassa rader medan dolda rader ignoreras
            worksheet.AutoFitRows(options);

            // Skriv ut radhöjderna
            Console.WriteLine("Row 0 height: " + worksheet.Cells.GetRowHeight(0));
            Console.WriteLine("Row 1 height: " + worksheet.Cells.GetRowHeight(1));
        }
    }
}
```

### Se även

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



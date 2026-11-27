---
title: "LoadOptions.AutoFitterOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions egenskap. Hämtar och anger alternativ för auto‑fitter"
type: docs
url: /sv/net/aspose.cells/loadoptions/autofitteroptions/
---
## LoadOptions.AutoFitterOptions property

Hämtar och anger alternativen för automatisk anpassning

```csharp
public AutoFitterOptions AutoFitterOptions { get; set; }
```

### Anmärkningar

Endast för xlsx‑, spreadsheetML‑fil nu.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Skapa AutoFitterOptions och ange egenskaper
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;
            options.OnlyAuto = false;

            // Skapa LoadOptions och tilldela AutoFitterOptions
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = options;

            // Läs in arbetsbok med de angivna alternativen
            Workbook workbook = new Workbook("example.xlsx", loadOptions);

            // Demonstrera auto‑fitting genom att hämta radens höjd
            double rowHeight = workbook.Worksheets[0].Cells.GetRowHeight(0);
            Console.WriteLine("Row height after auto-fitting: " + rowHeight);
        }
    }
}
```

### Se även

* class [AutoFitterOptions](../../autofitteroptions/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "AutoFitterOptions.ForRendering"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFitterOptions-egenskap. Anger om anpassning för renderingsändamål"
type: docs
url: /sv/net/aspose.cells/autofitteroptions/forrendering/
---
## AutoFitterOptions.ForRendering property

Anger om anpassning för renderingsändamål.

```csharp
public bool ForRendering { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyForRenderingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange exempeldata med lång text
            worksheet.Cells["A1"].PutValue("This is a long text that needs auto-fitting for rendering purposes.");
            
            // Skapa AutoFitterOptions och sätt ForRendering till true
            AutoFitterOptions options = new AutoFitterOptions();
            options.ForRendering = true;

            // Autoanpassa raden med hänsyn till rendering
            worksheet.AutoFitRows(0, 0, options);

            // Skriv ut den resulterande radhöjden i pixlar
            Console.WriteLine("Row height after auto-fitting (pixels): " + worksheet.Cells.GetRowHeightPixel(0));
        }
    }
}
```

### Se även

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



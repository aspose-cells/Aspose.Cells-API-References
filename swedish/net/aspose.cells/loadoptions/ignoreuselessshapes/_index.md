---
title: "LoadOptions.IgnoreUselessShapes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions-egenskap. Anger om onödiga former ska ignoreras"
type: docs
url: /sv/net/aspose.cells/loadoptions/ignoreuselessshapes/
---
## LoadOptions.IgnoreUselessShapes property

Anger om onödiga former ska ignoreras.

```csharp
public bool IgnoreUselessShapes { get; set; }
```

### Anmärkningar

Fungerar endast för xlsx, xlsb och xlsm-filer. Det finns många överlappande identiska former som är onödiga i vissa filer, vi kan ignorera dem vid inläsning av filer.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyIgnoreUselessShapesDemo
    {
        public static void Run()
        {
            // Skapa inläsningsalternativ och sätt IgnoreUselessShapes till true
            LoadOptions options = new LoadOptions();
            options.IgnoreUselessShapes = true;

            // Läs in arbetsboken med alternativen
            Workbook workbook = new Workbook("example.xlsx", options);

            // Skriv ut antalet former i det första kalkylbladet
            Console.WriteLine("Shapes count: " + workbook.Worksheets[0].Shapes.Count);
        }
    }
}
```

### Se även

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



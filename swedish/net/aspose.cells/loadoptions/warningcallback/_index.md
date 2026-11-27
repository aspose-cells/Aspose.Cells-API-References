---
title: "LoadOptions.WarningCallback"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions-egenskap. Hämtar eller anger varningsåteranrop"
type: docs
url: /sv/net/aspose.cells/loadoptions/warningcallback/
---
## LoadOptions.WarningCallback property

Hämtar eller anger varningsåteranrop.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning: {warningInfo.Description}");
        }
    }

    public class LoadOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Skapa ett anpassat varningsåteranrop
            IWarningCallback warningCallback = new CustomWarningCallback();

            // Initiera inläsningsalternativ med varningsåteranrop
            LoadOptions options = new LoadOptions();
            options.WarningCallback = warningCallback;
            options.IgnoreUselessShapes = true;

            // Läs in arbetsbok med alternativ
            Workbook workbook = new Workbook("example.xlsx", options);

            // Visa användning av varningsåteranrop genom att komma åt en cell
            Console.WriteLine($"Cell value: {workbook.Worksheets[0].Cells["A1"].StringValue}");

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* interface [IWarningCallback](../../iwarningcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



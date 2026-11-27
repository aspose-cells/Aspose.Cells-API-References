---
title: "TxtLoadOptions.IsMultiEncoded"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtLoadOptions egenskap. Sant betyder att filen innehåller flera kodningar"
type: docs
url: /sv/net/aspose.cells/txtloadoptions/ismultiencoded/
---
## TxtLoadOptions.IsMultiEncoded property

Sant betyder att filen innehåller flera kodningar.

```csharp
public bool IsMultiEncoded { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyIsMultiEncodedDemo
    {
        public static void Run()
        {
            // Skapa alternativ för textinläsning
            TxtLoadOptions options = new TxtLoadOptions();
            
            // Ställ in IsMultiEncoded till true för att hantera flera kodningar
            options.IsMultiEncoded = true;
            
            // Läs in arbetsboken med alternativen
            Workbook workbook = new Workbook("example.csv", options);
            
            // Visa exempelvärden från den inlästa filen
            Console.WriteLine("A2 Cell Value: " + workbook.Worksheets[0].Cells["A2"].StringValue);
            Console.WriteLine("A3 Cell Value: " + workbook.Worksheets[0].Cells["A3"].StringValue);
        }
    }
}
```

### Se även

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



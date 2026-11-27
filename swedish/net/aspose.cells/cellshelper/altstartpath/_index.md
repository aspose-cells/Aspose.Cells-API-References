---
title: "CellsHelper.AltStartPath"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper‑egenskap. Hämtar eller anger den alternativa startvägen som refereras till av vissa externa formelreferenser"
type: docs
url: /sv/net/aspose.cells/cellshelper/altstartpath/
---
## CellsHelper.AltStartPath property

Hämtar eller anger den alternativa startvägen, som refereras till av vissa externa formelreferenser.

```csharp
public static string AltStartPath { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyAltStartPathDemo
    {
        public static void Run()
        {
            // Ange den alternativa startvägen
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            
            // Ange också andra relevanta egenskaper för demonstration
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            
            // Visa sökvägarna för att demonstrera egenskapens användning
            Console.WriteLine("Main Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            
            // Exempel på hur dessa sökvägar kan användas
            Console.WriteLine("\nWhen resources aren't found in main path, system will check: " + CellsHelper.AltStartPath);
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



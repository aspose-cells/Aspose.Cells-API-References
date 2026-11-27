---
title: "CellsHelper.StartupPath"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-egenskap. Hämtar eller anger startvägen som refereras till av vissa externa formelreferenser"
type: docs
url: /sv/net/aspose.cells/cellshelper/startuppath/
---
## CellsHelper.StartupPath property

Hämtar eller anger startvägen, som refereras till av vissa externa formelreferenser.

```csharp
public static string StartupPath { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyStartupPathDemo
    {
        public static void Run()
        {
            // Ange startvägen
            CellsHelper.StartupPath = "C:\\Temp\\AsposeCellsStartup";
            
            // Visa startvägen
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);

            // Demonstrera ytterligare CellsHelper-egenskaper
            CellsHelper.SignificantDigits = 15;
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "CellsHelper.LibraryPath"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-egenskap. Hämtar eller anger sökvägen till biblioteket som refereras av vissa externa formelreferenser"
type: docs
url: /sv/net/aspose.cells/cellshelper/librarypath/
---
## CellsHelper.LibraryPath property

Hämtar eller anger bibliotekssökvägen som refereras till av vissa externa formelreferenser.

```csharp
public static string LibraryPath { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyLibraryPathDemo
    {
        public static void Run()
        {
            // Ange LibraryPath-egenskapen
            CellsHelper.LibraryPath = "C:\\MyLibraries\\AsposeCells";

            // Demonstrera hämtning och användning av LibraryPath
            Console.WriteLine("Current Library Path: " + CellsHelper.LibraryPath);

            // Exempel på att använda sökvägen i en filoperation
            string filePath = System.IO.Path.Combine(CellsHelper.LibraryPath, "test.xlsx");
            Console.WriteLine("Would load file from: " + filePath);
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Cells.CountLarge"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells‑egenskap. Hämtar det totala antalet instansierade Cell‑objekt"
type: docs
url: /sv/net/aspose.cells/cells/countlarge/
---
## Cells.CountLarge property

Hämtar det totala antalet instansierade Cell-objekt.

```csharp
public long CountLarge { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyCountLargeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite data i cellerna
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B2"].PutValue("World");
            worksheet.Cells["C3"].PutValue(123);
            
            // Demonstrera CountLarge‑egenskapen
            long cellCount = worksheet.Cells.CountLarge;
            Console.WriteLine($"Total cells in worksheet: {cellCount}");
            
            // Visa pappersstorlek för demonstration
            Console.WriteLine($"Paper Height: {worksheet.PageSetup.PaperHeight}");
            Console.WriteLine($"Paper Width: {worksheet.PageSetup.PaperWidth}");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



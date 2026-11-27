---
title: "Cells.StandardHeightPixels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar eller anger standardradhöjden i detta kalkylblad i pixlar."
type: docs
url: /sv/net/aspose.cells/cells/standardheightpixels/
---
## Cells.StandardHeightPixels property

Hämtar eller anger standardradshöjden i detta kalkylblad, i enheten pixlar.

```csharp
public int StandardHeightPixels { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightPixelsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange lite data i celler
            cells["A1"].PutValue("Sample Data");
            cells["B2"].PutValue(123);
            cells["C3"].PutValue(DateTime.Now);

            // Hämta standardhöjden i pixlar
            int standardHeight = cells.StandardHeightPixels;
            Console.WriteLine("Standard row height in pixels: " + standardHeight);

            // Visa radhöjder (ska matcha standardhöjden)
            for (int i = 0; i < 5; i++)
            {
                int rowHeight = cells.GetRowHeightPixel(i);
                Console.WriteLine($"Row {i} height: {rowHeight}px");
                Console.WriteLine($"Matches standard: {rowHeight == standardHeight}");
            }

            // Ändra standardhöjden och verifiera
            cells.StandardHeight = 20; // Set in points
            int newStandardHeight = cells.StandardHeightPixels;
            Console.WriteLine("\nNew standard height in pixels: " + newStandardHeight);

            // Verifiera att alla rader nu har den nya höjden
            for (int i = 0; i < 5; i++)
            {
                int rowHeight = cells.GetRowHeightPixel(i);
                Console.WriteLine($"Row {i} height: {rowHeight}px");
                Console.WriteLine($"Matches new standard: {rowHeight == newStandardHeight}");
            }
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Worksheet.GetSelectedAreas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet‑metod. Hämtar valda cellområden i designerns kalkylblad"
type: docs
url: /sv/net/aspose.cells/worksheet/getselectedareas/
---
## Worksheet.GetSelectedAreas method

Hämtar markerade cellområden i designerns kalkylblad.

```csharp
public Range[] GetSelectedAreas()
```

### Returvärde

Returnerar alla markerade områden.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetSelectedAreasDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Välj flera områden
            worksheet.SelectRange(0, 0, 2, 2, false); // First range (A1:C3)
            worksheet.SelectRange(4, 4, 6, 6, false); // Second range (E5:G7)
            
            // Hämta markerade områden
            Aspose.Cells.Range[] selectedAreas = worksheet.GetSelectedAreas();
            
            // Visa information om markerade områden
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            for (int i = 0; i < selectedAreas.Length; i++)
            {
                Console.WriteLine($"Area {i + 1}: {selectedAreas[i].Address}");
            }
            
            // Rensa markeringar och välj ett enda område
            worksheet.SelectRange(1, 1, 3, 3, true); // New single selection (B2:D4)
            
            // Hämta det enda markerade området
            selectedAreas = worksheet.GetSelectedAreas();
            Console.WriteLine("\nAfter single selection:");
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            Console.WriteLine("Selected area: " + selectedAreas[0].Address);
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



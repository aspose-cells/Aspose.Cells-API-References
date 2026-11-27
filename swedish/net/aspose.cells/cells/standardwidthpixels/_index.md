---
title: "Cells.StandardWidthPixels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar eller anger standardkolumnbredd i kalkylbladet i enhet pixlar."
type: docs
url: /sv/net/aspose.cells/cells/standardwidthpixels/
---
## Cells.StandardWidthPixels property

Hämtar eller anger standardkolumnbredden i kalkylbladet, i enheten pixlar.

```csharp
public int StandardWidthPixels { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthPixelsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in och hämta standardbredden i pixlar
            cells.StandardWidthPixels = 104;
            Console.WriteLine("Standard Width in Pixels: " + cells.StandardWidthPixels);

            // Ställ in och hämta standardbredden i tecken
            cells.StandardWidth = 12.375;
            Console.WriteLine("Standard Width in Characters: " + cells.StandardWidth);

            // Ställ in och hämta standardhöjden i punkter
            cells.StandardHeight = 14.25;
            Console.WriteLine("Standard Height in Points: " + cells.StandardHeight);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



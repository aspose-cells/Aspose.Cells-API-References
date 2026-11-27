---
title: "LineFormat.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LineFormat metod. Avgör om detta objekt har samma värde som ett annat specificerat LineFormat-objekt"
type: docs
url: /sv/net/aspose.cells.drawing/lineformat/equals/
---
## LineFormat.Equals method

Avgör om detta objekt har samma värde som ett annat specificerat [`LineFormat`](../) objekt.

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | Object | Det [`LineFormat`](../) objektet att jämföra med detta objekt. |

### Returvärde

Sant om värdet på parametern obj är detsamma som värdet på detta objekt; annars falskt. Om obj är null returnerar denna metod falskt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en linjeform i arbetsbladet
            worksheet.Shapes.AddLine(1, 1, 10, 10, 100, 0);
            
            // Hämta linjeformatet för den första formen
            LineFormat lineFmt1 = worksheet.Shapes[0].Line;
            LineFormat lineFmt2 = worksheet.Shapes[0].Line;
            
            // Jämför linjeformaten med metoden Equals
            if (lineFmt1.Equals((object)lineFmt2))
            {
                Console.WriteLine("The line formats are equal.");
            }
            else
            {
                Console.WriteLine("The line formats are not equal.");
            }
        }
    }
}
```

### Se även

* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



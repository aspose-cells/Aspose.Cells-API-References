---
title: "Range.MoveTo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range‑metod. Flytta det aktuella intervallet till destinationsintervallet"
type: docs
url: /sv/net/aspose.cells/range/moveto/
---
## Range.MoveTo method

Flyttar det aktuella området till destinationsområdet.

```csharp
public void MoveTo(int destRow, int destColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destRow | Int32 | Startraden för destinationsintervallet. |
| destColumn | Int32 | Startkolumnen för destinationsintervallet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodMoveToWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett exempelintervall (A1:B2)
            Aspose.Cells.Range originalRange = worksheet.Cells.CreateRange("A1", "B2");
            
            // Sätt in lite data i range för demonstration
            originalRange[0, 0].PutValue("A1");
            originalRange[0, 1].PutValue("B1");
            originalRange[1, 0].PutValue("A2");
            originalRange[1, 1].PutValue("B2");
            
            // Flytta range nedåt med 1 rad (till A2:B3)
            originalRange.MoveTo(originalRange.FirstRow + 1, originalRange.FirstColumn);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



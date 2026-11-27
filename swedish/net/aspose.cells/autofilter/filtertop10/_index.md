---
title: "AutoFilter.FilterTop10"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Filtrera de 10 bästa objekten i listan"
type: docs
url: /sv/net/aspose.cells/autofilter/filtertop10/
---
## AutoFilter.FilterTop10 method

Filtrera de 10 bästa objekten i listan

```csharp
public void FilterTop10(int fieldIndex, bool isTop, bool isPercent, int itemCount)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | Int32 | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstra fältet är fält 0). |
| isTop | Boolean | Anger om filtret är från toppen eller botten |
| isPercent | Boolean | Anger om objekten är i procent eller antal |
| itemCount | Int32 | Antalet objekt |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodFilterTop10WithInt32BooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata (5 rader x 3 kolumner med numeriska värden)
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Numbers");
            cells["A2"].PutValue(50);
            cells["A3"].PutValue(30);
            cells["A4"].PutValue(80);
            cells["A5"].PutValue(20);
            cells["A6"].PutValue(90);

            // Ställ in autofilterintervall
            worksheet.AutoFilter.Range = "A1:A6";

            // Tillämpa topp 10-filter (visar de 2 bästa objekten)
            worksheet.AutoFilter.FilterTop10(0, true, false, 2);

            // Uppdatera filtret
            worksheet.AutoFilter.Refresh();

            // Spara arbetsboken
            workbook.Save("FilterTop10Demo.xlsx");
        }
    }
}
```

### Se även

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



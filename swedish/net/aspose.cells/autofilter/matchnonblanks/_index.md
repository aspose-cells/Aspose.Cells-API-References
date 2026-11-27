---
title: "AutoFilter.MatchNonBlanks"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Matcha alla icke‑tomma celler i listan"
type: docs
url: /sv/net/aspose.cells/autofilter/matchnonblanks/
---
## AutoFilter.MatchNonBlanks method

Matcha alla icke-tomma celler i listan.

```csharp
public void MatchNonBlanks(int fieldIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | Int32 | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstra fältet är fält 0). |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodMatchNonBlanksWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata med några tomma celler
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(""); // Blank cell
            worksheet.Cells["B3"].PutValue(5);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(8);
            worksheet.Cells["A5"].PutValue(""); // Blank cell
            worksheet.Cells["B5"].PutValue(12);

            // Applicera autofilter för att bara visa icke‑tomma celler i kolumn A (index 0)
            worksheet.AutoFilter.Range = "A1:B5";
            worksheet.AutoFilter.MatchNonBlanks(0);
            worksheet.AutoFilter.Refresh();

            // Spara arbetsboken
            workbook.Save("FilterNonBlanks.xlsx");
        }
    }
}
```

### Se även

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "AutoFilter.MatchBlanks"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Matcha alla tomma celler i listan"
type: docs
url: /sv/net/aspose.cells/autofilter/matchblanks/
---
## AutoFilter.MatchBlanks method

Matcha alla tomma celler i listan.

```csharp
public void MatchBlanks(int fieldIndex)
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
    public class AutoFilterMethodMatchBlanksWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata med några tomma celler
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            // Lämna C2 tom
            
            worksheet.Cells["A3"].PutValue("Data3");
            // Lämna B3 tom
            worksheet.Cells["C3"].PutValue("Data6");
            
            // Applicera autofilter
            worksheet.AutoFilter.Range = "A1:C3";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Filtrera för att bara visa rader med tomma celler i kolumn 3 (C)
            filter.MatchBlanks(2); // Column index is 0-based
            
            // Uppdatera filtret
            filter.Refresh();
            
            // Spara arbetsboken
            workbook.Save("AutoFilterMatchBlanksDemo.xlsx");
        }
    }
}
```

### Se även

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



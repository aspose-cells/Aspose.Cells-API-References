---
title: "Cells.IsBlankColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Kontrollerar om given kolumn är tom och inte innehåller någon data"
type: docs
url: /sv/net/aspose.cells/cells/isblankcolumn/
---
## Cells.IsBlankColumn method

Kontrollerar om given kolumn är tom (innehåller ingen data).

```csharp
public bool IsBlankColumn(int columnIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | kolumnindexet |

### Returvärde

sant om den angivna kolumnen inte innehåller någon data

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsBlankColumnWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kontrollera om kolumn 2 är tom (ska vara sant för ett nytt kalkylblad)
            Console.WriteLine("Is column 2 blank? " + worksheet.Cells.IsBlankColumn(1));

            // Lägg till data i kolumn 2
            worksheet.Cells["B1"].PutValue("Test Data");

            // Kontrollera igen (ska nu vara falskt)
            Console.WriteLine("Is column 2 blank after adding data? " + worksheet.Cells.IsBlankColumn(1));

            // Skapa ett annat kalkylblad med helt tomma kolumner
            Worksheet worksheet2 = workbook.Worksheets.Add("BlankSheet");

            // Kontrollera en kolumn i det tomma kalkylbladet (ska vara sant)
            Console.WriteLine("Is column 3 blank in new sheet? " + worksheet2.Cells.IsBlankColumn(2));
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



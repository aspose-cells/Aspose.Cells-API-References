---
title: "Cells.GetLastDataRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar det sista radindexet för cellen som innehåller data i den angivna kolumnen"
type: docs
url: /sv/net/aspose.cells/cells/getlastdatarow/
---
## Cells.GetLastDataRow method

Hämtar det sista radindexet för cellen som innehåller data i den angivna kolumnen.

```csharp
public int GetLastDataRow(int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindex. |

### Returvärde

sista radindexet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetLastDataRowWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");
            
            // Hämta den sista dataraden i kolumn A (index 0)
            int lastRow = worksheet.Cells.GetLastDataRow(0);
            
            // Skriv ut resultatet
            Console.WriteLine("Last data row in column A: " + lastRow);
            
            // Infoga en ny rad efter den sista dataraden
            CellArea area = new CellArea();
            area.StartRow = lastRow + 1;
            area.EndRow = lastRow + 1;
            area.StartColumn = 0;
            area.EndColumn = 0;
            worksheet.Cells.InsertRange(area, 1, ShiftType.Down);
            
            // Lägg till data i den nya raden
            worksheet.Cells[lastRow + 2, 0].PutValue("New Data");
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



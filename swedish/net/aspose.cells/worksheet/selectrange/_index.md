---
title: "Worksheet.SelectRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Väljer ett område"
type: docs
url: /sv/net/aspose.cells/worksheet/selectrange/
---
## Worksheet.SelectRange method

Markerar ett område.

```csharp
public void SelectRange(int startRow, int startColumn, int totalRows, int totalColumns, 
    bool removeOthers)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startraden. |
| startColumn | Int32 | Startkolumnen |
| totalRows | Int32 | Antalet rader. |
| totalColumns | Int32 | Antalet kolumner |
| removeOthers | Boolean | True betyder att andra markerade områden tas bort och endast detta område väljs. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSelectRangeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Välj område från rad 1, kolumn 1 till rad 5, kolumn 5 (B2:F6) och gör det aktivt
            worksheet.SelectRange(1, 1, 5, 5, true);
            
            Console.WriteLine("Active cell: " + worksheet.ActiveCell);
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



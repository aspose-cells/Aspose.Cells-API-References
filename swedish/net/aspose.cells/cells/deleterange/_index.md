---
title: "Cells.DeleteRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Tar bort ett intervall av celler och flyttar celler enligt skiftalternativet"
type: docs
url: /sv/net/aspose.cells/cells/deleterange/
---
## Cells.DeleteRange method

Tar bort ett cellområde och flyttar celler enligt förskjutningsalternativet.

```csharp
public void DeleteRange(int startRow, int startColumn, int endRow, int endColumn, 
    ShiftType shiftType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startradindex. |
| startColumn | Int32 | Startkolumnindex. |
| endRow | Int32 | Slutradindex. |
| endColumn | Int32 | Slutkolumnindex. |
| shiftType | ShiftType | Flyttceller-alternativ. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRangeWithInt32Int32Int32Int32ShiftTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fyll i lite exempeldata
            sheet.Cells["A1"].PutValue("A1");
            sheet.Cells["B1"].PutValue("B1");
            sheet.Cells["C1"].PutValue("C1");
            sheet.Cells["A2"].PutValue("A2");
            sheet.Cells["B2"].PutValue("B2");
            sheet.Cells["C2"].PutValue("C2");

            // Ta bort intervall och flytta åt vänster
            sheet.Cells.DeleteRange(0, 1, 1, 2, ShiftType.Left);

            // Spara arbetsboken
            workbook.Save("DeleteRangeExample.xlsx");
        }
    }
}
```

### Se även

* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



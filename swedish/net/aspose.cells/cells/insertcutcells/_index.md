---
title: "Cells.InsertCutCells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Infoga klippt område"
type: docs
url: /sv/net/aspose.cells/cells/insertcutcells/
---
## Cells.InsertCutCells method

Infoga klippt område.

```csharp
public void InsertCutCells(Range cutRange, int row, int column, ShiftType shiftType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cutRange | Range | Det klippta området. |
| row | Int32 | Raden. |
| column | Int32 | Kolumnen. |
| shiftType | ShiftType | Anger hur andra objekt i målområdet ska förskjutas när ett klippt område infogas. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertCutCellsWithRangeInt32Int32ShiftTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet och dess celler
            Worksheet sourceSheet = workbook.Worksheets[0];
            Cells sourceCells = sourceSheet.Cells;
            
            // Lägg till lite data i källcellerna
            sourceCells["A1"].PutValue("Source A1");
            sourceCells["B1"].PutValue("Source B1");
            sourceCells["A2"].PutValue("Source A2");
            sourceCells["B2"].PutValue("Source B2");
            
            // Skapa ett andra kalkylblad som destination
            Worksheet destSheet = workbook.Worksheets.Add("Sheet2");
            Cells destCells = destSheet.Cells;
            
            // Lägg till lite initial data i destinationen
            destCells["A1"].PutValue("Dest A1");
            destCells["B1"].PutValue("Dest B1");
            
            // Skapa ett område att klippa (A1:B2 från källbladet)
            Aspose.Cells.Range cutRange = sourceCells.CreateRange("A1:B2");
            
            // Infoga de klippta cellerna på B2 i målbladet och flytta cellerna nedåt
            destCells.InsertCutCells(cutRange, 1, 1, ShiftType.Down);
            
            // Spara arbetsboken
            workbook.Save("InsertCutCellsDemo.xlsx");
            
            Console.WriteLine("InsertCutCells demo executed successfully.");
        }
    }
}
```

### Se även

* class [Range](../../range/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



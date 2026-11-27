---
title: "PivotFieldCollection.Move"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFieldCollection metod. Flyttar PivotField från aktuell position till destinationsposition"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldcollection/move/
---
## PivotFieldCollection.Move method

Flyttar PivotField från aktuell position till destinationspositionen

```csharp
public void Move(int currPos, int destPos)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| currPos | Int32 | Aktuell position för PivotField baserat på noll |
| destPos | Int32 | Destinationsposition för PivotField baserat på noll |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodMoveWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Skapa exempeldata
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 20;

            // Skapa pivottabell
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Lägg till fält i radområdet
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1);
            
            Console.WriteLine("Before move:");
            for (int i = 0; i < pivotTable.RowFields.Count; i++)
            {
                Console.WriteLine($"Field {i}: {pivotTable.RowFields[i].Name}");
            }
            
            // Flytta det första fältet till position 1
            pivotTable.RowFields.Move(0, 1);
            
            Console.WriteLine("\nAfter move:");
            for (int i = 0; i < pivotTable.RowFields.Count; i++)
            {
                Console.WriteLine($"Field {i}: {pivotTable.RowFields[i].Name}");
            }
        }
    }
}
```

### Se även

* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



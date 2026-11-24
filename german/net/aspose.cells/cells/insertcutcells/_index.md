---
title: "Cells.InsertCutCells"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Ausschnittbereich einfügen"
type: docs
url: /de/net/aspose.cells/cells/insertcutcells/
---
## Cells.InsertCutCells method

Einfügen des ausgeschnittenen Bereichs.

```csharp
public void InsertCutCells(Range cutRange, int row, int column, ShiftType shiftType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cutRange | Range | Der Ausschnittbereich. |
| row | Int32 | Die Zeile. |
| column | Int32 | Die Spalte. |
| shiftType | ShiftType | Gibt an, wie andere Objekte des Zielbereichs verschoben werden sollen, wenn ein cut range eingefügt wird. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertCutCellsWithRangeInt32Int32ShiftTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Auf das erste Arbeitsblatt und seine Zellen zugreifen
            Worksheet sourceSheet = workbook.Worksheets[0];
            Cells sourceCells = sourceSheet.Cells;
            
            // Füge einige Daten zu den Quellzellen hinzu
            sourceCells["A1"].PutValue("Source A1");
            sourceCells["B1"].PutValue("Source B1");
            sourceCells["A2"].PutValue("Source A2");
            sourceCells["B2"].PutValue("Source B2");
            
            // Erstelle ein zweites Arbeitsblatt als Ziel
            Worksheet destSheet = workbook.Worksheets.Add("Sheet2");
            Cells destCells = destSheet.Cells;
            
            // Füge einige Anfangsdaten zum Ziel hinzu
            destCells["A1"].PutValue("Dest A1");
            destCells["B1"].PutValue("Dest B1");
            
            // Erstelle einen Bereich zum Ausschneiden (A1:B2 vom Quellblatt)
            Aspose.Cells.Range cutRange = sourceCells.CreateRange("A1:B2");
            
            // Füge die cut cells bei B2 im Zielblatt ein und verschiebe die Zellen nach unten
            destCells.InsertCutCells(cutRange, 1, 1, ShiftType.Down);
            
            // Speichere die Arbeitsmappe
            workbook.Save("InsertCutCellsDemo.xlsx");
            
            Console.WriteLine("InsertCutCells demo executed successfully.");
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



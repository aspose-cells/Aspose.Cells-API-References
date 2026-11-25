---
title: "PivotFieldCollection.Move"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotFieldCollection. Sposta il PivotField dalla posizione corrente a quella di destinazione"
type: docs
url: /it/net/aspose.cells.pivot/pivotfieldcollection/move/
---
## PivotFieldCollection.Move method

Sposta il PivotField dalla posizione corrente a quella di destinazione

```csharp
public void Move(int currPos, int destPos)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| currPos | Int32 | Posizione corrente del PivotField basata su zero |
| destPos | Int32 | Posizione di destinazione del PivotField basata su zero |

### Esempi

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
            
            // Crea dati di esempio
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 20;

            // Crea tabella pivot
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Aggiungi campi all'area delle righe
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1);
            
            Console.WriteLine("Before move:");
            for (int i = 0; i < pivotTable.RowFields.Count; i++)
            {
                Console.WriteLine($"Field {i}: {pivotTable.RowFields[i].Name}");
            }
            
            // Sposta il primo campo alla posizione 1
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

### Vedi anche

* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



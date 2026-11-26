---
title: "PivotFieldCollection.Move"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotFieldCollection. Mueve el PivotField de la posición actual a la posición de destino"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldcollection/move/
---
## PivotFieldCollection.Move method

Mueve el PivotField de la posición actual a la posición de destino

```csharp
public void Move(int currPos, int destPos)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| currPos | Int32 | Posición actual del PivotField basada en cero |
| destPos | Int32 | Posición de destino del PivotField basada en cero |

### Ejemplos

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
            
            // Crear datos de ejemplo
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 20;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Agregar campos al área de filas
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1);
            
            Console.WriteLine("Before move:");
            for (int i = 0; i < pivotTable.RowFields.Count; i++)
            {
                Console.WriteLine($"Field {i}: {pivotTable.RowFields[i].Name}");
            }
            
            // Mover el primer campo a la posición 1
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

### Ver también

* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



---
title: "ValidationCollection.RemoveACell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ValidationCollection-Methode. Entfernt alle Validierungseinstellungen in der Zelle"
type: docs
url: /de/net/aspose.cells/validationcollection/removeacell/
---
## ValidationCollection.RemoveACell method

Entfernt alle Validierungseinstellungen in der Zelle.

```csharp
public void RemoveACell(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex der Zelle. |
| column | Int32 | Der Spaltenindex der Zelle. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodRemoveACellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie der Zelle A1 (Zeile 0, Spalte 0) eine Validierung hinzu
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            
            Validation validation = worksheet.Validations[worksheet.Validations.Add(area)];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Item1,Item2,Item3";

            // Entfernen Sie die Validierung aus der Zelle A1
            worksheet.Validations.RemoveACell(0, 0);

            Console.WriteLine("Validations count after removal: " + worksheet.Validations.Count);
        }
    }
}
```

### Siehe auch

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



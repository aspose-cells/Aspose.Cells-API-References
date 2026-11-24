---
title: "Validation.RemoveACell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validierungsmethode. Entfernen Sie die Validierungseinstellungen in der Zelle"
type: docs
url: /de/net/aspose.cells/validation/removeacell/
---
## Validation.RemoveACell method

Entfernt die Validierungseinstellungen in der Zelle.

```csharp
public void RemoveACell(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex. |
| column | Int32 | Der Spaltenindex. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodRemoveACellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Datenvalidierung zur ersten Zelle hinzufügen
            Validation validation = worksheet.Validations[0];
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            validation.Type = ValidationType.List;
            validation.Formula1 = "1,2,3";
            
            // Eine weitere Zelle zur Validierung hinzufügen
            validation.AddArea(new CellArea { StartRow = 1, StartColumn = 1, EndRow = 1, EndColumn = 1 });
            
            // Die zweite Zelle aus der Validierung entfernen
            validation.RemoveACell(1, 1);
            
            Console.WriteLine("Cell removed from validation successfully.");
        }
    }
}
```

### Siehe auch

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



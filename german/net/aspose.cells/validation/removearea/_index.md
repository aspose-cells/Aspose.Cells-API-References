---
title: "Validation.RemoveArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validierungsmethode. Entfernen Sie die Validierungseinstellungen im Bereich"
type: docs
url: /de/net/aspose.cells/validation/removearea/
---
## Validation.RemoveArea method

Entfernt die Validierungseinstellungen im Bereich.

```csharp
public void RemoveArea(CellArea cellArea)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellArea | CellArea | die Bereiche, in denen diese Validierungseinstellungen entfernt werden sollen. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodRemoveAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Validierung zum Arbeitsblatt hinzu
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "100";

            // Initialen Validierungsbereich hinzufügen
            CellArea initialArea = CellArea.CreateCellArea(0, 0, 0, 0);
            validation.AddArea(initialArea);

            // Einen weiteren Bereich zur Validierung hinzufügen
            CellArea additionalArea = CellArea.CreateCellArea(1, 1, 1, 1);
            validation.AddArea(additionalArea);

            Console.WriteLine("Validation areas count after adding: " + validation.Areas.Length);

            // Den zusätzlichen Bereich entfernen
            validation.RemoveArea(additionalArea);

            Console.WriteLine("Validation areas count after removing: " + validation.Areas.Length);

            // Mehrere Bereiche hinzufügen
            CellArea[] multipleAreas = new CellArea[]
            {
                CellArea.CreateCellArea(2, 2, 2, 2),
                CellArea.CreateCellArea(3, 3, 3, 3),
                CellArea.CreateCellArea(4, 4, 4, 4)
            };
            validation.AddAreas(multipleAreas, false, false);

            Console.WriteLine("Validation areas count after adding multiple: " + validation.Areas.Length);

            // Einen der Bereiche entfernen
            validation.RemoveArea(multipleAreas[1]);

            Console.WriteLine("Validation areas count after removing one: " + validation.Areas.Length);
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



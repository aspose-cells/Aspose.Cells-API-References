---
title: "ValidationCollection.RemoveArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ValidationCollection-Methode. Entfernt alle Validierungseinstellungen im Bereich"
type: docs
url: /de/net/aspose.cells/validationcollection/removearea/
---
## ValidationCollection.RemoveArea method

Entfernt alle Validierungseinstellungen im Bereich..

```csharp
public void RemoveArea(CellArea ca)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | CellArea | Der Bereich, der die Validierungseinstellungen enthält. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationCollectionMethodRemoveAreaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstellen Sie eine Validierung in einem bestimmten Bereich
            ValidationCollection validations = worksheet.Validations;
            CellArea validationArea = CellArea.CreateCellArea(0, 0, 5, 5);
            int validationIndex = validations.Add(validationArea);
            
            // Erstellen Sie einen Bereich, der aus der Validierung entfernt werden soll
            CellArea removeArea = CellArea.CreateCellArea(2, 2, 4, 4);
            
            try
            {
                // Rufen Sie die Methode RemoveArea mit dem Parameter CellArea auf
                validations.RemoveArea(removeArea);
                
                Console.WriteLine("Validation area removed successfully.");
                
                // Zeigen Sie die verbleibenden Validierungsbereiche an
                foreach (Validation validation in validations)
                {
                    if (validation.Areas.Length > 0)
                    {
                        Console.WriteLine($"Remaining validation area: {validation.Areas[0]}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("ValidationRemoveAreaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Validation.RemoveAreas"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Validierungsmethode. Entfernt diese Validierung aus den angegebenen Bereichen"
type: docs
url: /de/net/aspose.cells/validation/removeareas/
---
## Validation.RemoveAreas method

Entfernt diese Validierung aus den angegebenen Bereichen.

```csharp
public void RemoveAreas(CellArea[] areas)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereiche | CellArea[] | die Bereiche, in denen diese Validierungseinstellungen entfernt werden sollen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodRemoveAreasWithCellAreaArrayDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Datenvalidierung zum Arbeitsblatt hinzu
            int validationIndex = worksheet.Validations.Add();
            Validation validation = worksheet.Validations[validationIndex];
            
            // Validierungseinstellungen konfigurieren
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "1";
            validation.Formula2 = "10";

            // Zwei Zellbereiche für die Validierung erstellen
            CellArea area1 = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 1,
                EndColumn = 1
            };  // A1:B2
            CellArea area2 = new CellArea
            {
                StartRow = 2,
                StartColumn = 2,
                EndRow = 3,  // Original code had (2,2,1,1) which would be invalid endRow < startRow
                EndColumn = 3
            };  // C3:D4 (corrected end coordinates)
            
            // Bereiche zur Validierung hinzufügen
            validation.AddArea(area1);
            validation.AddArea(area2);
            Console.WriteLine($"Added areas: {validation.Areas.Length}");

            try
            {
                // Ein Array mit einem zu entfernenden Bereich erstellen
                CellArea[] removeAreas = { area1 };
                
                // RemoveAreas-Methode ausführen
                validation.RemoveAreas(removeAreas);
                Console.WriteLine($"Remaining areas after removal: {validation.Areas.Length}");
                
                // Koordinaten der verbleibenden Bereiche anzeigen
                foreach (CellArea remainingArea in validation.Areas)
                {
                    Console.WriteLine($"Area: {remainingArea.StartRow},{remainingArea.StartColumn} to {remainingArea.EndRow},{remainingArea.EndColumn}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Modifizierte Arbeitsmappe speichern
            workbook.Save("ValidationRemoveAreasDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



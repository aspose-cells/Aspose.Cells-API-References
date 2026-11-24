---
title: "SensitivityLabelCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SensitivityLabelCollection-Methode. Fügt ein Sensitivitätslabel hinzu"
type: docs
url: /de/net/aspose.cells.metas/sensitivitylabelcollection/add/
---
## SensitivityLabelCollection.Add method

Fügt ein Sensitivitätslabel hinzu.

```csharp
public int Add(string id, bool isEnabled, SensitivityLabelAssignmentType methodType, string siteId, 
    SensitivityLabelMarkType markType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| id | String | Die ID des Labels. |
| isEnabled | Boolean | Gibt an, ob dieses Sensitivitätslabel aktiviert ist. |
| methodType | SensitivityLabelAssignmentType | Der Zuweisungsmethodentyp. |
| siteId | String | Die ID der Site. |
| markType | SensitivityLabelMarkType | Der Markierungstyp. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelCollectionMethodAddWithStringBooleanSensitivityLabelADemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle eine neue SensitivityLabelCollection
            var sensitivityLabels = new SensitivityLabelCollection();
            
            try
            {
                // Rufe die Add-Methode mit spezifischen Parametern auf
                int index = sensitivityLabels.Add(
                    id: "Confidential",
                    isEnabled: true,
                    methodType: SensitivityLabelAssignmentType.Privileged,
                    siteId: "Contoso",
                    markType: SensitivityLabelMarkType.Watermark);
                
                Console.WriteLine($"Sensitivity label added at index: {index}");
                
                // Füge einige Daten hinzu, um die Wirkung zu demonstrieren
                worksheet.Cells["A1"].Value = "Confidential Data";
                worksheet.Cells["A2"].Value = "This document contains sensitive information";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("SensitivityLabelAddDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabelCollection](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)



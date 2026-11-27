---
title: "SensitivityLabelCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SensitivityLabelCollection-metod. Lägger till en känslighetsetikett"
type: docs
url: /sv/net/aspose.cells.metas/sensitivitylabelcollection/add/
---
## SensitivityLabelCollection.Add method

Lägger till en känslighetsetikett.

```csharp
public int Add(string id, bool isEnabled, SensitivityLabelAssignmentType methodType, string siteId, 
    SensitivityLabelMarkType markType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| id | String | Etikettens id. |
| isEnabled | Boolean | Anger om denna känslighetsetikett är aktiverad. |
| methodType | SensitivityLabelAssignmentType | Tilldelningsmetodens typ. |
| siteId | String | ID för webbplatsen. |
| markType | SensitivityLabelMarkType | Marktypen. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en ny SensitivityLabelCollection
            var sensitivityLabels = new SensitivityLabelCollection();
            
            try
            {
                // Anropa Add-metoden med specifika parametrar
                int index = sensitivityLabels.Add(
                    id: "Confidential",
                    isEnabled: true,
                    methodType: SensitivityLabelAssignmentType.Privileged,
                    siteId: "Contoso",
                    markType: SensitivityLabelMarkType.Watermark);
                
                Console.WriteLine($"Sensitivity label added at index: {index}");
                
                // Lägg till data för att demonstrera effekten
                worksheet.Cells["A1"].Value = "Confidential Data";
                worksheet.Cells["A2"].Value = "This document contains sensitive information";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("SensitivityLabelAddDemo.xlsx");
        }
    }
}
```

### Se även

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabelCollection](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)



---
title: "WorksheetCollection.SensitivityLabels"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Eigenschaft. Stellt alle Sensitivitätskennzeichnungen dar"
type: docs
url: /de/net/aspose.cells/worksheetcollection/sensitivitylabels/
---
## WorksheetCollection.SensitivityLabels property

Stellt alle Sensitivitätskennzeichnungen dar.

```csharp
public SensitivityLabelCollection SensitivityLabels { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metas;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertySensitivityLabelsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greift auf die Arbeitsblatt‑Sammlung zu
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Füge eine Sensitivitätskennzeichnung hinzu
            int index = worksheets.SensitivityLabels.Add(
                "{7e848398-70bd-400c-b8cf-2ab6f30d1b60}", // ID
                true,                                       // IsEnabled
                SensitivityLabelAssignmentType.Standard,     // AssignmentType
                "contoso-site",                             // SiteId
                SensitivityLabelMarkType.Header              // MarkType
            );
            
            // Überprüfe die hinzugefügte Kennzeichnung
            SensitivityLabel label = worksheets.SensitivityLabels[index];
            Console.WriteLine($"Label added - ID: {label.Id}, SiteID: {label.SiteId}");
            
            // Speichere die Arbeitsmappe
            workbook.Save("SensitivityLabelsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SensitivityLabelCollection](../../../aspose.cells.metas/sensitivitylabelcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



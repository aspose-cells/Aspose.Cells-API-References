---
title: "WorksheetCollection.SensitivityLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-egenskap. Representerar alla känslighetsetiketter"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/sensitivitylabels/
---
## WorksheetCollection.SensitivityLabels property

Representerar alla känslighetsetiketter.

```csharp
public SensitivityLabelCollection SensitivityLabels { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till arbetsbladsamlingen
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Lägg till en känslighetsetikett
            int index = worksheets.SensitivityLabels.Add(
                "{7e848398-70bd-400c-b8cf-2ab6f30d1b60}", // ID
                true,                                       // IsEnabled
                SensitivityLabelAssignmentType.Standard,     // AssignmentType
                "contoso-site",                             // SiteId
                SensitivityLabelMarkType.Header              // MarkType
            );
            
            // Verifiera den tillagda etiketten
            SensitivityLabel label = worksheets.SensitivityLabels[index];
            Console.WriteLine($"Label added - ID: {label.Id}, SiteID: {label.SiteId}");
            
            // Spara arbetsboken
            workbook.Save("SensitivityLabelsDemo.xlsx");
        }
    }
}
```

### Se även

* class [SensitivityLabelCollection](../../../aspose.cells.metas/sensitivitylabelcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



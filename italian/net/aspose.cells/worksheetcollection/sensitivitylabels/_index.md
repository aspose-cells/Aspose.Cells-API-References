---
title: "WorksheetCollection.SensitivityLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorksheetCollection proprietà. Rappresenta tutte le etichette di sensibilità"
type: docs
url: /it/net/aspose.cells/worksheetcollection/sensitivitylabels/
---
## WorksheetCollection.SensitivityLabels property

Rappresenta tutte le etichette di sensibilità.

```csharp
public SensitivityLabelCollection SensitivityLabels { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alla collezione di fogli di lavoro
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Aggiungi un'etichetta di sensibilità
            int index = worksheets.SensitivityLabels.Add(
                "{7e848398-70bd-400c-b8cf-2ab6f30d1b60}", // ID
                true,                                       // IsEnabled
                SensitivityLabelAssignmentType.Standard,     // AssignmentType
                "contoso-site",                             // SiteId
                SensitivityLabelMarkType.Header              // MarkType
            );
            
            // Verifica l'etichetta aggiunta
            SensitivityLabel label = worksheets.SensitivityLabels[index];
            Console.WriteLine($"Label added - ID: {label.Id}, SiteID: {label.SiteId}");
            
            // Salva la cartella di lavoro
            workbook.Save("SensitivityLabelsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SensitivityLabelCollection](../../../aspose.cells.metas/sensitivitylabelcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



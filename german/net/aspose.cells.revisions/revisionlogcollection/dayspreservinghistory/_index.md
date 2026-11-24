---
title: "RevisionLogCollection.DaysPreservingHistory"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionLogCollection‑Eigenschaft. Gibt die Anzahl der Tage zurück und legt sie fest, für die die Tabellenkalkulationsanwendung die Änderungsverlauf für diese Arbeitsmappe aufbewahrt"
type: docs
url: /de/net/aspose.cells.revisions/revisionlogcollection/dayspreservinghistory/
---
## RevisionLogCollection.DaysPreservingHistory property

Liest und setzt die Anzahl der Tage, die die Tabellenkalkulationsanwendung die Änderungshistorie für diese Arbeitsmappe aufbewahrt.

```csharp
public int DaysPreservingHistory { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionPropertyDaysPreservingHistoryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Value");
            
            // Setze die DaysPreservingHistory‑Eigenschaft
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 40;
            
            string outputPath = "output_DaysPreservingHistory.xlsx";
            workbook.Save(outputPath);
            
            // Lade neu, um die Eigenschaft zu überprüfen
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("DaysPreservingHistory: " + 
                loadedWorkbook.Worksheets.RevisionLogs.DaysPreservingHistory);
        }
    }
}
```

### Siehe auch

* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)



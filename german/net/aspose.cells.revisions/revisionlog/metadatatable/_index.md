---
title: "RevisionLog.MetadataTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionLog-Eigenschaft. Gibt die Tabelle zurück, die Metadaten über eine Liste spezifischer Änderungen enthält, die an dieser Arbeitsmappe vorgenommen wurden"
type: docs
url: /de/net/aspose.cells.revisions/revisionlog/metadatatable/
---
## RevisionLog.MetadataTable property

Ermittelt die Tabelle, die Metadaten über eine Liste spezifischer Änderungen enthält, die für diese Arbeitsmappe vorgenommen wurden.

```csharp
public RevisionHeader MetadataTable { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogPropertyMetadataTableDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Nehmen Sie einige Änderungen vor, um eine Revisionshistorie zu erstellen
            worksheet.Cells["A1"].PutValue("Original Value");
            workbook.Save("RevisionDemo.xlsx", SaveFormat.Xlsx);
            
            // Zelle ändern, um eine Revision zu erstellen
            worksheet.Cells["A1"].PutValue("Modified Value");
            workbook.Save("RevisionDemo_modified.xlsx", SaveFormat.Xlsx);

            // Öffnen Sie die geänderte Arbeitsmappe erneut, um auf Revisionsprotokolle zuzugreifen
            workbook = new Workbook("RevisionDemo_modified.xlsx");
            
            // Zugriff auf Revisionsprotokolle
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            
            if (revisionLogs.Count > 0)
            {
                RevisionLog revisionLog = revisionLogs[0];
                RevisionHeader metadata = revisionLog.MetadataTable;
                
                Console.WriteLine("Revision Metadata:");
                Console.WriteLine("Saved Time: " + metadata.SavedTime);
                Console.WriteLine("Modified By: " + metadata.UserName);
                Console.WriteLine("Number of Revisions: " + revisionLog.Revisions.Count);
            }
            else
            {
                Console.WriteLine("No revision history found");
            }
        }
    }
}
```

### Siehe auch

* class [RevisionHeader](../../revisionheader/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)



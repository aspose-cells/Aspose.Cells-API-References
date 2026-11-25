---
title: "RevisionLog.MetadataTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionLog. Ottiene la tabella che contiene i metadati su un elenco di modifiche specifiche avvenute per questa cartella di lavoro"
type: docs
url: /it/net/aspose.cells.revisions/revisionlog/metadatatable/
---
## RevisionLog.MetadataTable property

Ottiene la tabella che contiene i metadati su un elenco di modifiche specifiche avvenute per questa cartella di lavoro.

```csharp
public RevisionHeader MetadataTable { get; }
```

### Esempi

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
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Apporta alcune modifiche per creare la cronologia delle revisioni
            worksheet.Cells["A1"].PutValue("Original Value");
            workbook.Save("RevisionDemo.xlsx", SaveFormat.Xlsx);
            
            // Modifica la cella per creare una revisione
            worksheet.Cells["A1"].PutValue("Modified Value");
            workbook.Save("RevisionDemo_modified.xlsx", SaveFormat.Xlsx);

            // Riapri la cartella di lavoro modificata per accedere ai registri di revisione
            workbook = new Workbook("RevisionDemo_modified.xlsx");
            
            // Accedi ai log delle revisioni
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

### Vedi anche

* class [RevisionHeader](../../revisionheader/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)



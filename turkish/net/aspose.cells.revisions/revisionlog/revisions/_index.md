---
title: "RevisionLog.Revisions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionLog özelliği. Bu günlükteki tüm revizyonları alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisionlog/revisions/
---
## RevisionLog.Revisions property

Bu günlükteki tüm revizyonları alır.

```csharp
public RevisionCollection Revisions { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogPropertyRevisionsDemo
    {
        public static void Run()
        {
            // Revizyon geçmişiyle bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Revizyonları izlemek için bazı değişiklikler yapın
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].Formula = "=A2*2";
            
            // Revizyon takibiyle kaydedin
            workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
            
            // Revizyonlar oluşturmak için daha fazla değişiklik yapın
            worksheet.Cells["A1"].PutValue("Modified Value");
            worksheet.Cells["A2"].PutValue(200);
            
            // Revizyonları kaydetmek için tekrar kaydedin
            workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
            
            // Revizyonlu çalışma kitabını yükleyin
            Workbook workbookWithRevisions = new Workbook("revision_demo.xlsx");
            
            // Revizyon günlüklerine erişin
            RevisionLogCollection revisionLogs = workbookWithRevisions.Worksheets.RevisionLogs;
            
            // Her revizyon günlüğünü işleyin
            foreach (RevisionLog log in revisionLogs)
            {
                Console.WriteLine($"Processing revision log with {log.Revisions.Count} revisions");
                
                // Revizyon koleksiyonuna erişin
                RevisionCollection revisions = log.Revisions;
                
                foreach (Revision revision in revisions)
                {
                    Console.WriteLine($"Revision Type: {revision.Type}");
                    
                    if (revision.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange cellChange = (RevisionCellChange)revision;
                        Console.WriteLine($"Cell {cellChange.CellName} changed from '{cellChange.OldValue}' to '{cellChange.NewValue}'");
                    }
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [RevisionCollection](../../revisioncollection/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)



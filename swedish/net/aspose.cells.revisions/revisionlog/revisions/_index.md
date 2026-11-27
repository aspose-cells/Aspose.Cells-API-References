---
title: "RevisionLog.Revisions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionLog-egenskap. Hämtar alla revisioner i denna logg"
type: docs
url: /sv/net/aspose.cells.revisions/revisionlog/revisions/
---
## RevisionLog.Revisions property

Hämtar alla revisioner i den här loggen.

```csharp
public RevisionCollection Revisions { get; }
```

### Exempel

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
            // Skapa en arbetsbok med revisionshistorik
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Gör några ändringar för att spåra revisioner
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].Formula = "=A2*2";
            
            // Spara med revisionsspårning
            workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
            
            // Gör fler ändringar för att skapa revisioner
            worksheet.Cells["A1"].PutValue("Modified Value");
            worksheet.Cells["A2"].PutValue(200);
            
            // Spara igen för att registrera revisioner
            workbook.Save("revision_demo.xlsx", SaveFormat.Xlsx);
            
            // Läs in arbetsboken med revisioner
            Workbook workbookWithRevisions = new Workbook("revision_demo.xlsx");
            
            // Kom åt revisionsloggar
            RevisionLogCollection revisionLogs = workbookWithRevisions.Worksheets.RevisionLogs;
            
            // Bearbeta varje revisionslogg
            foreach (RevisionLog log in revisionLogs)
            {
                Console.WriteLine($"Processing revision log with {log.Revisions.Count} revisions");
                
                // Åtkomst till revisionssamlingen
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

### Se även

* class [RevisionCollection](../../revisioncollection/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)



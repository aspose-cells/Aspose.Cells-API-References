---
title: "RevisionInsertDelete.Revisions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionInsertDelete-egenskapen. Hämtar revisionslistan för denna operation"
type: docs
url: /sv/net/aspose.cells.revisions/revisioninsertdelete/revisions/
---
## RevisionInsertDelete.Revisions property

Hämtar revisionslistan för denna operation.

```csharp
public RevisionCollection Revisions { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertDeletePropertyRevisionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och aktivera revisionsspårning
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30;

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Utför operationer för att generera revisioner
            worksheet.Cells.InsertRows(0, 1);
            worksheet.Cells.DeleteRows(1, 1);

            // Hämta revisionsloggarna
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Iterera genom alla revisionsloggar
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionInsertDelete)
                    {
                        RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                        // Åtkomst till Revisions-egenskapen (skrivskyddad)
                        RevisionCollection revisions = revisionInsertDelete.Revisions;

                        // Visa information om revisionerna
                        Console.WriteLine("Revision Type: " + revisionInsertDelete.Type);
                        Console.WriteLine("Action Type: " + revisionInsertDelete.ActionType);
                        Console.WriteLine("Cell Area: " + revisionInsertDelete.CellArea);
                        Console.WriteLine("Number of related revisions: " + revisions.Count);

                        // Demonstrera användning av Revisions-samlingen
                        foreach (Revision relatedRevision in revisions)
                        {
                            Console.WriteLine(" - Related revision ID: " + relatedRevision.Id);
                            if (relatedRevision is RevisionInsertDelete)
                            {
                                RevisionInsertDelete relatedInsertDelete = (RevisionInsertDelete)relatedRevision;
                                Console.WriteLine("   Action Type: " + relatedInsertDelete.ActionType);
                                Console.WriteLine("   Cell Area: " + relatedInsertDelete.CellArea);
                            }
                        }
                    }
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionInsertDeletePropertyRevisionsDemo.xlsx");
        }
    }
}
```

### Se även

* class [RevisionCollection](../../revisioncollection/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)



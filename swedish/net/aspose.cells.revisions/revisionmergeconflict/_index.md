---
title: "Klass RevisionMergeConflict"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.RevisionMergeConflict-klass. Representerar en revisionspost som indikerar att det fanns en sammanslagningskonflikt"
type: docs
url: /sv/net/aspose.cells.revisions/revisionmergeconflict/
---
## RevisionMergeConflict class

Representerar en revisionspost som indikerar att det fanns en sammanslagningskonflikt.

```csharp
public class RevisionMergeConflict : Revision
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Hämtar numret för denna revision.(Arv från [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionmergeconflict/type/) { get; } | Hämtar typen av revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Hämtar kalkylbladet.(Arv från [`Revision`](../revision/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionsClassRevisionMergeConflictDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gör några ändringar för att skapa revisionshistorik
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue("Another Value");

            // Spara arbetsboken för att generera revisioner
            workbook.Save("RevisionMergeConflictDemo_Before.xlsx");

            // Skapa ett scenario med sammanslagningskonflikt
            worksheet.Cells["A1"].PutValue("Conflicting Change 1");
            worksheet.Cells["A1"].PutValue("Conflicting Change 2");

            // Hämta revisionshistoriken (iterera direkt genom RevisionLogCollection)
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Hitta och demonstrera RevisionMergeConflict
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionMergeConflict mergeConflict)
                    {
                        // Demonstrera åtkomst till revisionstypen
                        RevisionType revisionType = mergeConflict.Type;
                    }
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionMergeConflictDemo_After.xlsx");
        }
    }
}
```

### Se även

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)



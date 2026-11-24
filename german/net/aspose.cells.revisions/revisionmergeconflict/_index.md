---
title: "Klasse RevisionMergeConflict"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.RevisionMergeConflict Klasse. Stellt einen Revisionsdatensatz dar, der anzeigt, dass ein Zusammenführungs‑Konflikt aufgetreten ist"
type: docs
url: /de/net/aspose.cells.revisions/revisionmergeconflict/
---
## RevisionMergeConflict class

Stellt einen Revisionsdatensatz dar, der anzeigt, dass ein Merge-Konflikt aufgetreten ist.

```csharp
public class RevisionMergeConflict : Revision
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ermittelt die Nummer dieser Revision.(Vererbt von [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionmergeconflict/type/) { get; } | Liest den Typ der Revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ermittelt das Arbeitsblatt.(Vererbt von [`Revision`](../revision/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionsClassRevisionMergeConflictDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Nehmen Sie einige Änderungen vor, um eine Revisionshistorie zu erstellen
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue("Another Value");

            // Speichern Sie die Arbeitsmappe, um Revisionen zu erzeugen
            workbook.Save("RevisionMergeConflictDemo_Before.xlsx");

            // Erstellen Sie ein Szenario für einen Merge-Konflikt
            worksheet.Cells["A1"].PutValue("Conflicting Change 1");
            worksheet.Cells["A1"].PutValue("Conflicting Change 2");

            // Rufen Sie die Revisionshistorie ab (iterieren Sie direkt durch RevisionLogCollection)
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Finden und demonstrieren Sie RevisionMergeConflict
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionMergeConflict mergeConflict)
                    {
                        // Demonstrieren Sie den Zugriff auf den Revisionstyp
                        RevisionType revisionType = mergeConflict.Type;
                    }
                }
            }

            // Speichern Sie die Arbeitsmappe mit Revisionen
            workbook.Save("RevisionMergeConflictDemo_After.xlsx");
        }
    }
}
```

### Siehe auch

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)



---
title: "Klasse RevisionLog"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.RevisionLog Klasse. Stellt das Revisionsprotokoll dar"
type: docs
url: /de/net/aspose.cells.revisions/revisionlog/
---
## RevisionLog class

Stellt das Revisionsprotokoll dar.

```csharp
public class RevisionLog
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [MetadataTable](../../aspose.cells.revisions/revisionlog/metadatatable/) { get; } | Ermittelt die Tabelle, die Metadaten über eine Liste spezifischer Änderungen enthält, die für diese Arbeitsmappe vorgenommen wurden. |
| [Revisions](../../aspose.cells.revisions/revisionlog/revisions/) { get; } | Ermittelt alle Revisionen in diesem Protokoll. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionLogDemo
    {
        public static void RevisionLogExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Greifen Sie auf die Revisionsprotokolle der Arbeitsmappe zu
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Prüfe, ob Revisionseinträge vorhanden sind
            if (revisionLogs.Count > 0)
            {
                // Greifen Sie auf das erste Revisionsprotokoll zu
                RevisionLog revisionLog = revisionLogs[0];

                // Greifen Sie auf die Metadaten‑Tabelle des Revisionsprotokolls zu
                RevisionHeader metadataTable = revisionLog.MetadataTable;

                // Greifen Sie auf die Revisionen im Revisionsprotokoll zu
                RevisionCollection revisions = revisionLog.Revisions;

                // Zeigen Sie einige Informationen zu den Revisionen an
                Console.WriteLine("Number of revisions: " + revisions.Count);
                Console.WriteLine("Metadata Table: " + metadataTable.ToString());
            }
            else
            {
                Console.WriteLine("No revision logs found.");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("RevisionLogExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)



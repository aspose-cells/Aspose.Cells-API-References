---
title: "RevisionInsertDelete.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionInsertDelete-Eigenschaft. Stellt den Typ der Revision dar"
type: docs
url: /de/net/aspose.cells.revisions/revisioninsertdelete/type/
---
## RevisionInsertDelete.Type property

Stellt den Typ der Revision dar.

```csharp
public override RevisionType Type { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertDeletePropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch und aktiviere die Versionsverfolgung
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30; // Enable revision tracking by setting days

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Zeile ein, um einen Revisionsdatensatz zu erzeugen
            worksheet.Cells.InsertRows(0, 1);

            // Rufe die Revisionssammlung ab (RevisionLogCollection selbst ist die Sammlung)
            RevisionLogCollection revisions = workbook.Worksheets.RevisionLogs;

            // Finde das RevisionInsertDelete in den Revisionen
            foreach (RevisionLog revisionLog in revisions)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionInsertDelete)
                    {
                        RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                        // Den Wert der Type-Eigenschaft anzeigen
                        Console.WriteLine("Revision Type: " + revisionInsertDelete.Type);

                        // Demonstrieren Sie die Verwendung der Type-Eigenschaft
                        if (revisionInsertDelete.Type == RevisionType.InsertDelete)
                        {
                            Console.WriteLine("This revision represents an insert/delete operation");
                            Console.WriteLine("Affected cell area: " + revisionInsertDelete.CellArea);
                            Console.WriteLine("Action type: " + revisionInsertDelete.ActionType);
                        }

                        break;
                    }
                }
            }

            // Speichern Sie die Arbeitsmappe mit Revisionen
            workbook.Save("RevisionInsertDeletePropertyTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)



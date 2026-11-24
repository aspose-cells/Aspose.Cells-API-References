---
title: "RevisionLogCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionLogCollection-Eigenschaft. Gibt RevisionLog nach Index zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisionlogcollection/item/
---
## RevisionLogCollection indexer

Gibt [`RevisionLog`](../../revisionlog/) nach Index zurück.

```csharp
public RevisionLog this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Rückgabewert

Gibt das [`RevisionLog`](../../revisionlog/)-Objekt zurück.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionLogCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Gemeinsames Arbeitsbuch aktivieren, um Revisionen zu unterstützen
            workbook.Settings.Shared = true;

            // Greife auf die Sammlung der Revisionsprotokolle zu
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            try
            {
                // Prüfe, ob Revisionseinträge vorhanden sind
                if (revisionLogs.Count > 0)
                {
                    // Greifen Sie über die Item-Eigenschaft auf das erste Revisionsprotokoll zu
                    RevisionLog firstLog = revisionLogs[0];

                    // Grundlegende Informationen zum Revisionsprotokoll anzeigen
                    Console.WriteLine("First revision log accessed via Item property:");
                    Console.WriteLine($"Revision count: {firstLog.Revisions.Count}");
                }
                else
                {
                    Console.WriteLine("No revision logs available in the workbook.");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("RevisionLogItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [RevisionLog](../../revisionlog/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)



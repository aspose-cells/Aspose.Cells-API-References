---
title: "Klasse Revision"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.Revision Klasse. Stellt die Revision dar"
type: docs
url: /de/net/aspose.cells.revisions/revision/
---
## Revision class

Stellt die Revision dar.

```csharp
public abstract class Revision
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Gibt die Nummer dieser Revision zurück. |
| virtual [Type](../../aspose.cells.revisions/revision/type/) { get; } | Stellt den Typ der Revision dar. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Gibt das Arbeitsblatt zurück. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Füge einige Daten hinzu, um möglicherweise Revisionen zu erzeugen
                worksheet.Cells["A1"].PutValue("Original Value");

                // Speichere die Arbeitsmappe, um eine Basislinie festzulegen
                workbook.Save("RevisionDemo_Baseline.xlsx");

                // Lade die Arbeitsmappe und führe eine Änderung durch
                Workbook modifiedWorkbook = new Workbook("RevisionDemo_Baseline.xlsx");
                modifiedWorkbook.Worksheets[0].Cells["A1"].PutValue("Modified Value");

                // Prüfe, ob Revisionseinträge vorhanden sind
                if (modifiedWorkbook.Worksheets.RevisionLogs.Count > 0)
                {
                    RevisionLog log = modifiedWorkbook.Worksheets.RevisionLogs[0];
                    if (log.Revisions.Count > 0)
                    {
                        // Hole die erste Revision
                        Revision revision = log.Revisions[0];

                        // Zeige schreibgeschützte Eigenschaften an
                        Console.WriteLine($"Revision ID: {revision.Id}");
                        Console.WriteLine($"Revision Type: {revision.Type}");
                        Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");

                        // Speichere die geänderte Arbeitsmappe
                        modifiedWorkbook.Save("RevisionDemo_Modified.xlsx");
                    }
                    else
                    {
                        Console.WriteLine("No revisions found in the log");
                    }
                }
                else
                {
                    Console.WriteLine("No revision logs available");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with Revision: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)



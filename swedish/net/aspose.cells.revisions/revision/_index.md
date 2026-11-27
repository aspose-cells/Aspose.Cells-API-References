---
title: "Klass Revision"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.Revision-klass. Representerar revisionen"
type: docs
url: /sv/net/aspose.cells.revisions/revision/
---
## Revision class

Representerar revisionen.

```csharp
public abstract class Revision
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Hämtar numret för denna revision. |
| virtual [Type](../../aspose.cells.revisions/revision/type/) { get; } | Representerar typen av revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Hämtar kalkylbladet. |

### Exempel

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
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till lite data för att eventuellt skapa revisioner
                worksheet.Cells["A1"].PutValue("Original Value");

                // Spara arbetsboken för att etablera en grundlinje
                workbook.Save("RevisionDemo_Baseline.xlsx");

                // Läs in arbetsboken och gör en ändring
                Workbook modifiedWorkbook = new Workbook("RevisionDemo_Baseline.xlsx");
                modifiedWorkbook.Worksheets[0].Cells["A1"].PutValue("Modified Value");

                // Kontrollera om det finns några revisionsloggar
                if (modifiedWorkbook.Worksheets.RevisionLogs.Count > 0)
                {
                    RevisionLog log = modifiedWorkbook.Worksheets.RevisionLogs[0];
                    if (log.Revisions.Count > 0)
                    {
                        // Hämta den första revisionen
                        Revision revision = log.Revisions[0];

                        // Visa skrivskyddade egenskaper
                        Console.WriteLine($"Revision ID: {revision.Id}");
                        Console.WriteLine($"Revision Type: {revision.Type}");
                        Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");

                        // Spara den modifierade arbetsboken
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

### Se även

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)



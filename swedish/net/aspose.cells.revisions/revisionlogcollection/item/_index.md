---
title: "RevisionLogCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionLogCollection-egenskap. Hämtar RevisionLog efter index"
type: docs
url: /sv/net/aspose.cells.revisions/revisionlogcollection/item/
---
## RevisionLogCollection indexer

Hämtar [`RevisionLog`](../../revisionlog/) efter index.

```csharp
public RevisionLog this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

Returnerar [`RevisionLog`](../../revisionlog/) objekt.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Aktivera delad arbetsbok för att stödja revisioner
            workbook.Settings.Shared = true;

            // Åtkomst till revisionsloggssamlingen
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            try
            {
                // Kontrollera om det finns några revisionsloggar
                if (revisionLogs.Count > 0)
                {
                    // Kom åt den första revisionsloggen med Item-egenskapen
                    RevisionLog firstLog = revisionLogs[0];

                    // Visa grundläggande information om revisionsloggen
                    Console.WriteLine("First revision log accessed via Item property:");
                    Console.WriteLine($"Revision count: {firstLog.Revisions.Count}");
                }
                else
                {
                    Console.WriteLine("No revision logs available in the workbook.");
                }

                // Spara arbetsboken
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

### Se även

* class [RevisionLog](../../revisionlog/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)



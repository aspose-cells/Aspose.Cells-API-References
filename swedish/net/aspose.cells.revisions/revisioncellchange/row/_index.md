---
title: "RevisionCellChange.Row"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellChange egenskap. Hämtar radindex för cellen"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellchange/row/
---
## RevisionCellChange.Row property

Hämtar radindex för cellen.

```csharp
public int Row { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till initial data för att skapa en revision
            worksheet.Cells["B5"].PutValue("Original Value");

            // Modifiera cellen för att skapa en revision
            worksheet.Cells["B5"].PutValue("Modified Value");

            try
            {
                // Åtkomst till revisionsloggarna
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                foreach (RevisionLog log in revisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCellChange cellChange)
                        {
                            // Visa värdet för egenskapen Row
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Row Index: " + cellChange.Row);
                            Console.WriteLine("Column Index: " + cellChange.Column);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // Demonstrera användning av Row-egenskapen
                            if (cellChange.Row >= 0)
                            {
                                Console.WriteLine("\nThe revision occurred in row " +
                                    (cellChange.Row + 1) + " (1-based index)");
                            }
                        }
                    }
                }

                // Spara arbetsboken
                workbook.Save("RevisionCellChangePropertyRowDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)



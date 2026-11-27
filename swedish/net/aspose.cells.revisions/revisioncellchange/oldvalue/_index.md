---
title: "RevisionCellChange.OldValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellChange-egenskap. Hämtar det gamla värdet för cellen"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellchange/oldvalue/
---
## RevisionCellChange.OldValue property

Hämtar det gamla värdet för cellen.

```csharp
public object OldValue { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyOldValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till initial data för att skapa en revision
            worksheet.Cells["A1"].PutValue("Original Value");

            // Modifiera cellen för att skapa en revision
            worksheet.Cells["A1"].PutValue("Modified Value");

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
                            // Visa värdet för egenskapen OldValue
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // Demonstrera användning av egenskapen OldValue
                            if (cellChange.OldValue != null)
                            {
                                Console.WriteLine("\nThe cell was previously set to: " + cellChange.OldValue);
                            }
                        }
                    }
                }

                // Spara arbetsboken
                workbook.Save("RevisionCellChangePropertyOldValueDemo.xlsx");
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



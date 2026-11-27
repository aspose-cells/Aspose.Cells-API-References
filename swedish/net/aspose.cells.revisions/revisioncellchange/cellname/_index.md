---
title: "RevisionCellChange.CellName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellChange-egenskap. Hämtar namnet på cellen"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellchange/cellname/
---
## RevisionCellChange.CellName property

Hämtar cellens namn.

```csharp
public string CellName { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyCellNameDemo
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
                            // Visa värdet för egenskapen CellName
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Row Index: " + cellChange.Row);
                            Console.WriteLine("Column Index: " + cellChange.Column);

                            // Demonstrera användning av egenskapen CellName
                            if (cellChange.CellName == "A1")
                            {
                                Console.WriteLine("\nThe revision is for cell A1");
                                Console.WriteLine("Old Value: " + cellChange.OldValue);
                                Console.WriteLine("New Value: " + cellChange.NewValue);
                            }
                        }
                    }
                }

                // Spara arbetsboken
                workbook.Save("RevisionCellChangePropertyCellNameDemo.xlsx");
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



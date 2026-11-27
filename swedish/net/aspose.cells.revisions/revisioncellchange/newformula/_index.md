---
title: "RevisionCellChange.NewFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellChange egenskap. Hämtar den gamla formeln"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellchange/newformula/
---
## RevisionCellChange.NewFormula property

Hämtar den gamla formeln.

```csharp
public string NewFormula { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyNewFormulaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med revisionsspårning
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in initial formel i cell A1
            worksheet.Cells["A1"].Formula = "=SUM(B1:B3)";
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Ändra formeln för att skapa en revision
            worksheet.Cells["A1"].Formula = "=AVERAGE(B1:B3)";

            // Åtkomst till revisionsloggarna
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange && cellChange.CellName == "A1")
                    {
                        // Visa information om formelförändring
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Formula: " + cellChange.OldFormula);
                        Console.WriteLine("New Formula: " + cellChange.NewFormula);
                        Console.WriteLine("Old Value: " + cellChange.OldValue);
                        Console.WriteLine("New Value: " + cellChange.NewValue);

                        // Demonstrera användning av NewFormula-egenskapen
                        if (!string.IsNullOrEmpty(cellChange.NewFormula))
                        {
                            Console.WriteLine("\nThe cell's new formula calculates: " + 
                                worksheet.Cells["A1"].StringValue);
                        }
                    }
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionCellChangePropertyNewFormulaDemo.xlsx");
        }
    }
}
```

### Se även

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)



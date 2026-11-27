---
title: "RevisionCellChange.Column"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellChange-egenskap. Hämtar kolumnindex för cellen"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellchange/column/
---
## RevisionCellChange.Column property

Hämtar kolumnindex för cellen.

```csharp
public int Column { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med revisionsspårning
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ändra cell B2 för att generera en revision
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Initial Value");

            // Ändra cellen för att skapa en revision
            cell.PutValue("Modified Value");

            // Åtkomst till revisionsloggarna
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // Visa kolumninformation från revisionen
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Column Index: " + cellChange.Column);
                        Console.WriteLine("Row Index: " + cellChange.Row);

                        // Demonstrera användning av egenskapen Column
                        if (cellChange.Column == 1) // Column B is index 1
                        {
                            Console.WriteLine("\nThis revision affects column B");
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);
                        }
                    }
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionCellChangePropertyColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)



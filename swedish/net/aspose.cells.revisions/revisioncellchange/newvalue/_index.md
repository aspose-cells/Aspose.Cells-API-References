---
title: "RevisionCellChange.NewValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellChange egenskap. Hämtar cellens nya värde"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellchange/newvalue/
---
## RevisionCellChange.NewValue property

Hämtar det nya värdet för cellen.

```csharp
public object NewValue { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyNewValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till initial data i cell A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");

            // Modifiera cellen för att skapa en revision
            cell.PutValue("Modified Value");

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
                            // Visa NewValue-egenskapen
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // Demonstrera användning av NewValue-egenskapen
                            if (cellChange.NewValue != null)
                            {
                                Console.WriteLine("\nThe new value is: " + cellChange.NewValue.ToString());
                            }
                        }
                    }
                }

                // Spara arbetsboken med revisioner
                workbook.Save("RevisionCellChangePropertyNewValueDemo.xlsx");
                Console.WriteLine("\nWorkbook saved with revisions.");
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



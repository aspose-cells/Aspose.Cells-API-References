---
title: "RevisionCellChange.IsNewFormatted"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellChange-egenskap. Anger om denna cell är nyformaterad"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellchange/isnewformatted/
---
## RevisionCellChange.IsNewFormatted property

Indikerar om denna cell är nyformaterad.

```csharp
public bool IsNewFormatted { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyIsNewFormattedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med revisionsspårning
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in initialt cellvärde och stil
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Initial Value");
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.Name = "Arial";
            initialStyle.Font.Size = 10;
            cell.SetStyle(initialStyle);

            // Ändra cellvärdet och stilen för att skapa en revision
            cell.PutValue("Updated Value");
            Style newStyle = workbook.CreateStyle();
            newStyle.Font.Name = "Calibri";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            cell.SetStyle(newStyle);

            // Åtkomst till revisionsloggarna
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // Visa revisionsinformation
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Value: " + cellChange.OldValue);
                        Console.WriteLine("New Value: " + cellChange.NewValue);

                        // Demonstrera egenskapen IsNewFormatted
                        Console.WriteLine("\nFormatting Information:");
                        Console.WriteLine("IsOldFormatted: " + cellChange.IsOldFormatted);
                        Console.WriteLine("IsNewFormatted: " + cellChange.IsNewFormatted);

                        if (cellChange.IsNewFormatted)
                        {
                            Console.WriteLine("The cell has new formatting applied in this revision.");
                            Console.WriteLine("New Font: " + cellChange.NewStyle.Font.Name);
                            Console.WriteLine("New Font Size: " + cellChange.NewStyle.Font.Size);
                            Console.WriteLine("Is Bold: " + cellChange.NewStyle.Font.IsBold);
                        }
                    }
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionCellChangePropertyIsNewFormattedDemo.xlsx");
        }
    }
}
```

### Se även

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)



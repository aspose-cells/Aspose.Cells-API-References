---
title: "RevisionCellChange.NewStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellChange-egenskap. Hämtar den nya stilen för cellen"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellchange/newstyle/
---
## RevisionCellChange.NewStyle property

Hämtar den nya stilen för cellen.

```csharp
public Style NewStyle { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyNewStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med revisionsspårning
            Workbook workbook = new Workbook();
            // Ingen direkt StartTrackingRevisions-metod tillgänglig - revisioner spåras automatiskt
            Worksheet worksheet = workbook.Worksheets[0];

            // Modifiera en cell för att generera en revision
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");
            Style originalStyle = workbook.CreateStyle();
            originalStyle.Font.Name = "Arial";
            originalStyle.Font.Size = 10;
            cell.SetStyle(originalStyle);

            // Ändra cellen för att skapa en revision
            cell.PutValue("New Value");
            Style newStyle = workbook.CreateStyle();
            newStyle.Font.Name = "Times New Roman";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            cell.SetStyle(newStyle);

            // Ingen direkt StopTrackingRevisions-metod tillgänglig

            // Åtkomst till revisionsloggen via RevisionLogs istället för Revisions
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // Visa information om celländringsrevisionen
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Value: " + cellChange.OldValue);
                        Console.WriteLine("New Value: " + cellChange.NewValue);

                        // Åtkomst till NewStyle-egenskapen
                        Style revisionNewStyle = cellChange.NewStyle;
                        Console.WriteLine("\nNew Style Properties:");
                        Console.WriteLine("Font Name: " + revisionNewStyle.Font.Name);
                        Console.WriteLine("Font Size: " + revisionNewStyle.Font.Size);
                        Console.WriteLine("Is Bold: " + revisionNewStyle.Font.IsBold);
                    }
                }
            }

            // Spara arbetsboken med revisioner
            workbook.Save("RevisionCellChangePropertyNewStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../../aspose.cells/style/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)



---
title: "Cells.MergedCells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar samlingen av sammanslagna celler"
type: docs
url: /sv/net/aspose.cells/cells/mergedcells/
---
## Cells.MergedCells property

Hämtar samlingen av sammanslagna celler.

```csharp
[Obsolete("Use Cells.GetMergedAreas() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList MergedCells { get; }
```

### Anmärkningar

I den här samlingen är varje objekt en [`CellArea`](../../cellarea/) struktur som representerar ett område av sammanslagna celler.

OBS: Den här metoden är nu föråldrad. Använd istället Cells.GetMergedAreas()‑metoden. Denna metod kommer att tas bort 12 månader senare, från och med november 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsPropertyMergedCellsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Slå samman celler i två olika områden
            cells.Merge(0, 0, 2, 2); // Merges A1:B2
            cells.Merge(2, 2, 2, 2); // Merges C3:D4

            // Åtkomst till MergedCells‑egenskapen (skrivskyddad)
            ArrayList mergedRanges = cells.MergedCells;

            // Visa initiala antalet sammanslagna celler och områden
            Console.WriteLine($"Initial merged cells count: {mergedRanges.Count}");
            foreach (CellArea area in mergedRanges)
            {
                Console.WriteLine($"Merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
            }

            // Dela upp det första sammanslagna området
            cells.UnMerge(0, 0, 2, 2);

            // Visa uppdaterat antal sammanslagna celler och områden
            Console.WriteLine($"\nAfter unmerging A1:B2 - Merged cells count: {cells.MergedCells.Count}");
            foreach (CellArea area in cells.MergedCells)
            {
                Console.WriteLine($"Remaining merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
            }

            // Spara resultatet
            workbook.Save("PropertyMergedCellsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



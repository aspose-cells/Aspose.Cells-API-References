---
title: "Cell.IsStyleSet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Anger om cellens stil är inställd. Om den returnerar false betyder det att den här cellen har ett standardcellformat"
type: docs
url: /sv/net/aspose.cells/cell/isstyleset/
---
## Cell.IsStyleSet property

Anger om cellens stil är angiven. Om den returnerar false betyder det att cellen har ett standardformat.

```csharp
public bool IsStyleSet { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsStyleSetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Åtkomst till en cell som ännu inte har stylats
            Cell unsetStyleCell = cells["A1"];
            Console.WriteLine($"Cell A1 IsStyleSet before styling: {unsetStyleCell.IsStyleSet}");

            // Styla en annan cell
            Cell styledCell = cells["B2"];
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            styledCell.SetStyle(style);

            Console.WriteLine($"Cell B2 IsStyleSet after styling: {styledCell.IsStyleSet}");

            // Kontrollera om stil ärvs från raden
            Row row = cells.Rows[4];
            row.SetStyle(style);
            Cell rowInheritedCell = cells["E4"];
            Console.WriteLine($"Cell E4 IsStyleSet (inherited from row): {rowInheritedCell.IsStyleSet}");

            // Ställ explicit in stil till null för en cell
            Cell nullStyleCell = cells["C3"];
            nullStyleCell.SetStyle(null);
            Console.WriteLine($"Cell C3 IsStyleSet after setting null: {nullStyleCell.IsStyleSet}");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Column.HasCustomStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Kolumnegenskap. Anger om den här kolumnen har anpassade stilinställningar som skiljer sig från standardinställningarna som ärvs från arbetsboken"
type: docs
url: /sv/net/aspose.cells/column/hascustomstyle/
---
## Column.HasCustomStyle property

Indikerar om den här kolumnen har anpassade stilinställningar (annorlunda än standardinställningen som ärvs från arbetsboken).

```csharp
public bool HasCustomStyle { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till den första kolumnen
            Column column = worksheet.Cells.Columns[0];

            // Visa initialt HasCustomState‑värde
            Console.WriteLine("Initial HasCustomStyle: " + column.HasCustomStyle);

            // Ändra kolumnstil för att demonstrera ändring av HasCustomStyle
            Style columnStyle = column.GetStyle();
            columnStyle.BackgroundColor = Color.LightBlue;
            column.SetStyle(columnStyle);

            // Visa uppdaterat HasCustomStyle‑värde
            Console.WriteLine("After style modification - HasCustomStyle: " + column.HasCustomStyle);

            // Skapa en annan kolumn med standardstil för jämförelse
            Column secondColumn = worksheet.Cells.Columns[1];
            Console.WriteLine("Second column HasCustomStyle: " + secondColumn.HasCustomStyle);

            // Spara arbetsboken
            workbook.Save("ColumnHasCustomStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



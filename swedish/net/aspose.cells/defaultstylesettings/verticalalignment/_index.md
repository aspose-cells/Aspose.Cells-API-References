---
title: "DefaultStyleSettings.VerticalAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Egenskapen DefaultStyleSettings. Hämtar/Anger standardvärdet för vertikal justering"
type: docs
url: /sv/net/aspose.cells/defaultstylesettings/verticalalignment/
---
## DefaultStyleSettings.VerticalAlignment property

Hämtar/Anger standardvärdet för vertikal justering

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ange standard vertikal justering till Botten
            LoadOptions options = new LoadOptions();
            options.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange några exempeldata
            worksheet.Cells["A1"].PutValue("Sample Text 1");
            worksheet.Cells["B1"].PutValue("Sample Text 2");
            worksheet.Cells["C1"].PutValue("Sample Text 3");

            // Verifiera att den vertikala justeringen tillämpas på alla celler
            foreach (Cell cell in worksheet.Cells)
            {
                Console.WriteLine($"Cell {cell.Name} Vertical Alignment: {cell.GetStyle().VerticalAlignment}");
            }

            // Spara arbetsboken
            workbook.Save("VerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Klass ColorFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ColorFilter-klass. Representerar inställning för att filtrera intervallet efter färg."
type: docs
url: /sv/net/aspose.cells/colorfilter/
---
## ColorFilter class

Representerar inställning för att filtrera området efter färg.

```csharp
public class ColorFilter
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [FilterByFillColor](../../aspose.cells/colorfilter/filterbyfillcolor/) { get; set; } | Om filtrering efter cellens fyllningsfärg. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetColor](../../aspose.cells/colorfilter/getcolor/)(WorksheetCollection) | Hämtar färgen för detta filter. |

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassColorFilterDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata med olika färger.
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Red");
            cells["A2"].PutValue("Green");
            cells["A3"].PutValue("Blue");
            cells["A4"].PutValue("Red");
            
            // Applicera färger på celler.
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = Color.Red;
            style1.Pattern = BackgroundType.Solid;
            cells["A1"].SetStyle(style1);
            cells["A4"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = Color.Green;
            style2.Pattern = BackgroundType.Solid;
            cells["A2"].SetStyle(style2);
            
            Style style3 = workbook.CreateStyle();
            style3.ForegroundColor = Color.Blue;
            style3.Pattern = BackgroundType.Solid;
            cells["A3"].SetStyle(style3);
            
            // Skapa autofilter
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Skapa färgfilter för röda celler.
            CellsColor cr = workbook.CreateCellsColor();
            cr.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, cr, cr);
            filter.Refresh();
            
            // Kontrollera filtrerade rader.
            Console.WriteLine("Row 1 hidden: " + cells.IsRowHidden(0));
            Console.WriteLine("Row 2 hidden: " + cells.IsRowHidden(1));
            Console.WriteLine("Row 3 hidden: " + cells.IsRowHidden(2));
            Console.WriteLine("Row 4 hidden: " + cells.IsRowHidden(3));
            
            // Åtkomst till färgfilter
            FilterColumn fc = filter.FilterColumns[0];
            ColorFilter cf = fc.Filter as ColorFilter;
            
            Console.WriteLine("Filter by fill color: " + cf.FilterByFillColor);
            Console.WriteLine("Filter color: " + cf.GetColor(workbook.Worksheets));
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



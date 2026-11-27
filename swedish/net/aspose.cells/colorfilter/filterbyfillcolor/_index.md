---
title: "ColorFilter.FilterByFillColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ColorFilter-egenskap. Huruvida filtrera efter cellens fyllningsfärg"
type: docs
url: /sv/net/aspose.cells/colorfilter/filterbyfillcolor/
---
## ColorFilter.FilterByFillColor property

Om filtrering efter cellens fyllningsfärg.

```csharp
public bool FilterByFillColor { get; set; }
```

### Anmärkningar

Sant: cellens fyllningsfärg; Falskt: cellens teckensnittsfärg.

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColorFilterPropertyFilterByFillColorDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata med olika fyllningsfärger
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A3"].PutValue("Data2");
            cells["A4"].PutValue("Data3");

            // Ange fyllningsfärger
            Style style1 = cells["A2"].GetStyle();
            style1.ForegroundColor = Color.Red;
            style1.Pattern = BackgroundType.Solid;
            cells["A2"].SetStyle(style1);

            Style style2 = cells["A3"].GetStyle();
            style2.ForegroundColor = Color.Blue;
            style2.Pattern = BackgroundType.Solid;
            cells["A3"].SetStyle(style2);

            Style style3 = cells["A4"].GetStyle();
            style3.ForegroundColor = Color.Green;
            style3.Pattern = BackgroundType.Solid;
            cells["A4"].SetStyle(style3);

            // Applicera autofilter
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;

            // Skapa färgfilter för fyllningsfärg
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, null);
            filter.Refresh();

            // Verifiera filterinställningar
            FilterColumn filterColumn = filter.FilterColumns[0];
            ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
            
            // Demonstrera FilterByFillColor-egenskapen
            Console.WriteLine("FilterByFillColor: " + colorFilter.FilterByFillColor); // Should be True
            Console.WriteLine("Filtered rows:");
            for (int row = 1; row <= 3; row++)
            {
                Console.WriteLine($"Row {row} hidden: {cells.IsRowHidden(row)}");
            }
        }
    }
}
```

### Se även

* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "AutoFilter.AddFontColorFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Lägger till ett teckensnittsfärgsfilter"
type: docs
url: /sv/net/aspose.cells/autofilter/addfontcolorfilter/
---
## AutoFilter.AddFontColorFilter method

Lägger till ett teckensnittsfärgsfilter.

```csharp
public void AddFontColorFilter(int fieldIndex, CellsColor color)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | Int32 | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstra fältet är fält 0). |
| color | CellsColor | Objektet [`CellsColor`](../../cellscolor/). |

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFontColorFilterWithInt32CellsColorDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata med olika teckensnittsfärger
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Item 1");
            cells["A3"].PutValue("Item 2");
            cells["A4"].PutValue("Item 3");
            
            // Ange teckensnittsfärger
            Style style = cells["A2"].GetStyle();
            style.Font.Color = Color.Red;
            cells["A2"].SetStyle(style);
            
            style = cells["A3"].GetStyle();
            style.Font.Color = Color.Blue;
            cells["A3"].SetStyle(style);
            
            style = cells["A4"].GetStyle();
            style.Font.Color = Color.Green;
            cells["A4"].SetStyle(style);

            // Applicera autofilter
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Skapa färgfilter för röd text
            CellsColor cr = workbook.CreateCellsColor();
            cr.Color = Color.Red;
            
            // Lägg till teckensnittsfärgfilter
            filter.AddFontColorFilter(0, cr);
            filter.Refresh();
            
            // Spara arbetsboken
            workbook.Save("AutoFilterFontColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellsColor](../../cellscolor/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



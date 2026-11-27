---
title: "ColorFilter.GetColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ColorFilter‑metod. Hämtar färgen på detta filter"
type: docs
url: /sv/net/aspose.cells/colorfilter/getcolor/
---
## ColorFilter.GetColor method

Hämtar färgen för detta filter.

```csharp
public Color GetColor(WorksheetCollection sheets)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheets | WorksheetCollection |  |

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColorFilterMethodGetColorWithWorksheetCollectionDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["A4"].PutValue("Item 3");
            
            // Skapa autofilter
            worksheet.AutoFilter.Range = "A1:A4";
            
            // Skapa färgfilter
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            worksheet.AutoFilter.Refresh();
            
            // Hämta färgfilter och verifiera dess färg
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
            
            if (colorFilter != null)
            {
                Color retrievedColor = colorFilter.GetColor(workbook.Worksheets);
                Console.WriteLine("Filter color: " + retrievedColor.ToString());
            }
        }
    }
}
```

### Se även

* class [WorksheetCollection](../../worksheetcollection/)
* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



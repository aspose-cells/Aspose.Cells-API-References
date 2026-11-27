---
title: "Enum FilterType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.FilterType enum. Filtertypen"
type: docs
url: /sv/net/aspose.cells/filtertype/
---
## FilterType enumeration

Filtertypen.

```csharp
public enum FilterType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| ColorFilter | `0` | Filtrera efter fyllningsfärg i cellen. |
| CustomFilters | `1` | Anpassad filtertyp. |
| DynamicFilter | `2` | Dynamisk filtertyp. |
| MultipleFilters | `3` | När flera värden väljs att filtreras på, eller när en grupp datumvärden väljs att filtreras på, grupperar detta element dessa kriterier tillsammans. |
| IconFilter | `4` | Filtrera efter ikon för villkorsstyrd formatering. |
| Top10 | `5` | Topp 10‑filter. |
| None | `6` | Inget filter. |

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFilterTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Color");
            worksheet.Cells["A2"].PutValue("Red");
            worksheet.Cells["A3"].PutValue("Green");
            worksheet.Cells["A4"].PutValue("Blue");
            
            // Skapa autofilter
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Skapa färgfilter
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            
            // Lägg till färgfilter i kolumnen
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            filter.Refresh();
            
            // Kontrollera filtertyp
            FilterColumn filterColumn = filter.FilterColumns[0];
            Console.WriteLine("Filter Type: " + filterColumn.FilterType);
            
            // Verifiera egenskaperna för färgfilter
            if (filterColumn.FilterType == FilterType.ColorFilter)
            {
                ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
                Console.WriteLine("Filter by fill color: " + colorFilter.FilterByFillColor);
                Console.WriteLine("Filter color: " + colorFilter.GetColor(workbook.Worksheets));
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



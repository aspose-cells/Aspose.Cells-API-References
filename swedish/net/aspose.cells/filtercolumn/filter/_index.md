---
title: "FilterColumn.Filter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FilterColumn egenskap. Hämtar och anger villkoret för filtrering av data"
type: docs
url: /sv/net/aspose.cells/filtercolumn/filter/
---
## FilterColumn.Filter property

Hämtar och anger villkoret för filtrering av data.

```csharp
[Obsolete("Use corresponding property according to the filter type instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public object Filter { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället motsvarande egenskap enligt [`FilterType`](../filtertype/). Och för filtertypen MultipleFilters är det returnerade objektet nu [`FilterValueCollection`](../../filtervaluecollection/) istället för [`MultipleFilterCollection`](../../multiplefiltercollection/). Denna egenskap kommer att tas bort 12 månader senare från och med oktober 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFilterDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata med färgformatering
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Color");
            cells["A2"].PutValue("Red");
            cells["A3"].PutValue("Red");
            cells["A4"].PutValue("Blue");
            
            // Formatera celler med färger
            Style redStyle = workbook.CreateStyle();
            redStyle.ForegroundColor = Color.Red;
            redStyle.Pattern = BackgroundType.Solid;
            
            Style blueStyle = workbook.CreateStyle();
            blueStyle.ForegroundColor = Color.Blue;
            blueStyle.Pattern = BackgroundType.Solid;
            
            cells["A2"].SetStyle(redStyle);
            cells["A3"].SetStyle(redStyle);
            cells["A4"].SetStyle(blueStyle);
            
            // Applicera autofilter
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Lägg till färgfilter för röda celler
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            filter.Refresh();
            
            // Åtkomst till filterkolumnen och dess Filter-egenskap
            FilterColumn fc = filter.FilterColumns[0];
            ColorFilter cf = fc.Filter as ColorFilter;
            
            // Skriv ut filteregenskaper
            Console.WriteLine($"Filter type: {fc.FilterType}");
            Console.WriteLine($"Filter by fill color: {cf.FilterByFillColor}");
            Console.WriteLine($"Filter color: {cf.GetColor(workbook.Worksheets)}");
            
            // Spara arbetsboken
            workbook.Save("ColorFilterDemo.xlsx");
        }
    }
}
```

### Se även

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



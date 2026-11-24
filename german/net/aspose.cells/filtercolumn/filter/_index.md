---
title: "FilterColumn.Filter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FilterColumn-Eigenschaft. Gibt die Bedingung zum Filtern von Daten zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells/filtercolumn/filter/
---
## FilterColumn.Filter property

Liest und setzt die Bedingung für das Filtern von Daten.

```csharp
[Obsolete("Use corresponding property according to the filter type instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public object Filter { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die entsprechende Eigenschaft gemäß [`FilterType`](../filtertype/). Und für den Filtertyp MultipleFilters ist das zurückgegebene Objekt jetzt [`FilterValueCollection`](../../filtervaluecollection/) anstelle von [`MultipleFilterCollection`](../../multiplefiltercollection/). Diese Eigenschaft wird 12 Monate später, seit Oktober 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

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
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten mit Farbformatierung hinzufügen
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Color");
            cells["A2"].PutValue("Red");
            cells["A3"].PutValue("Red");
            cells["A4"].PutValue("Blue");
            
            // Zellen mit Farben formatieren
            Style redStyle = workbook.CreateStyle();
            redStyle.ForegroundColor = Color.Red;
            redStyle.Pattern = BackgroundType.Solid;
            
            Style blueStyle = workbook.CreateStyle();
            blueStyle.ForegroundColor = Color.Blue;
            blueStyle.Pattern = BackgroundType.Solid;
            
            cells["A2"].SetStyle(redStyle);
            cells["A3"].SetStyle(redStyle);
            cells["A4"].SetStyle(blueStyle);
            
            // Auto-Filter anwenden
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Farbfilter für rote Zellen hinzufügen
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            filter.Refresh();
            
            // Zugriff auf die Filterspalte und deren Filter-Eigenschaft
            FilterColumn fc = filter.FilterColumns[0];
            ColorFilter cf = fc.Filter as ColorFilter;
            
            // Filtereigenschaften ausgeben
            Console.WriteLine($"Filter type: {fc.FilterType}");
            Console.WriteLine($"Filter by fill color: {cf.FilterByFillColor}");
            Console.WriteLine($"Filter color: {cf.GetColor(workbook.Worksheets)}");
            
            // Speichere die Arbeitsmappe
            workbook.Save("ColorFilterDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



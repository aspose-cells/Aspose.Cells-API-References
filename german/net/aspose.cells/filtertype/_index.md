---
title: "Enum FilterType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FilterType enum. Der Filtertyp"
type: docs
url: /de/net/aspose.cells/filtertype/
---
## FilterType enumeration

Der Filtertyp.

```csharp
public enum FilterType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| ColorFilter | `0` | Filtern nach Füllfarbe der Zelle. |
| CustomFilters | `1` | Benutzerdefinierter Filtertyp. |
| DynamicFilter | `2` | Dynamischer Filtertyp. |
| MultipleFilters | `3` | Wenn mehrere Werte zum Filtern ausgewählt werden oder wenn eine Gruppe von Datumswerten zum Filtern ausgewählt wird, gruppiert dieses Element diese Kriterien zusammen. |
| IconFilter | `4` | Filtern nach Symbol der bedingten Formatierung. |
| Top10 | `5` | Top‑10-Filter. |
| None | `6` | Kein Filter. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Color");
            worksheet.Cells["A2"].PutValue("Red");
            worksheet.Cells["A3"].PutValue("Green");
            worksheet.Cells["A4"].PutValue("Blue");
            
            // Automatischen Filter erstellen
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Farbfilter erstellen
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            
            // Farbfilter zur Spalte hinzufügen
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            filter.Refresh();
            
            // Filtertyp prüfen
            FilterColumn filterColumn = filter.FilterColumns[0];
            Console.WriteLine("Filter Type: " + filterColumn.FilterType);
            
            // Die Eigenschaften des Farbfilters überprüfen
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

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



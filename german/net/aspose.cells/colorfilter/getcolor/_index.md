---
title: "ColorFilter.GetColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ColorFilter-Methode. Gibt die Farbe dieses Filters zurück"
type: docs
url: /de/net/aspose.cells/colorfilter/getcolor/
---
## ColorFilter.GetColor method

Ermittelt die Farbe dieses Filters.

```csharp
public Color GetColor(WorksheetCollection sheets)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Blätter | WorksheetCollection |  |

### Beispiele

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
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["A4"].PutValue("Item 3");
            
            // Automatischen Filter erstellen
            worksheet.AutoFilter.Range = "A1:A4";
            
            // Farbfilter erstellen
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            worksheet.AutoFilter.Refresh();
            
            // Holen Sie den Farbfilter und überprüfen Sie seine Farbe
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

### Siehe auch

* class [WorksheetCollection](../../worksheetcollection/)
* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



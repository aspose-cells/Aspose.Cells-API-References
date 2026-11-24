---
title: "AutoFilter.AddFontColorFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter-Methode. Fügt einen Schriftfarbenfilter hinzu"
type: docs
url: /de/net/aspose.cells/autofilter/addfontcolorfilter/
---
## AutoFilter.AddFontColorFilter method

Fügt einen Schriftfarbenfilter hinzu.

```csharp
public void AddFontColorFilter(int fieldIndex, CellsColor color)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | Int32 | Der ganzzahlige Versatz des Feldes, auf dem der Filter basieren soll (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| color | CellsColor | Das [`CellsColor`](../../cellscolor/) Objekt. |

### Beispiele

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
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten mit unterschiedlichen Schriftfarben hinzufügen
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Item 1");
            cells["A3"].PutValue("Item 2");
            cells["A4"].PutValue("Item 3");
            
            // Schriftfarben festlegen
            Style style = cells["A2"].GetStyle();
            style.Font.Color = Color.Red;
            cells["A2"].SetStyle(style);
            
            style = cells["A3"].GetStyle();
            style.Font.Color = Color.Blue;
            cells["A3"].SetStyle(style);
            
            style = cells["A4"].GetStyle();
            style.Font.Color = Color.Green;
            cells["A4"].SetStyle(style);

            // Auto-Filter anwenden
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Farbfilter für rote Schrift erstellen
            CellsColor cr = workbook.CreateCellsColor();
            cr.Color = Color.Red;
            
            // Schriftfarbenfilter hinzufügen
            filter.AddFontColorFilter(0, cr);
            filter.Refresh();
            
            // Speichere die Arbeitsmappe
            workbook.Save("AutoFilterFontColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellsColor](../../cellscolor/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



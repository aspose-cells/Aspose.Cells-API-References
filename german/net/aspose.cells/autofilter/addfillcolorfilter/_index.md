---
title: "AutoFilter.AddFillColorFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter-Methode. Fügt einen Füllfarbfilter hinzu"
type: docs
url: /de/net/aspose.cells/autofilter/addfillcolorfilter/
---
## AutoFilter.AddFillColorFilter method

Fügt einen Füllfarbenfilter hinzu.

```csharp
public void AddFillColorFilter(int fieldIndex, BackgroundType pattern, CellsColor foregroundColor, 
    CellsColor backgroundColor)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | Int32 | Der ganzzahlige Versatz des Feldes, auf dem der Filter basieren soll (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| pattern | BackgroundType | Der Hintergrundmuster-Typ. |
| foregroundColor | CellsColor | Die Vordergrundfarbe. |
| backgroundColor | CellsColor | Die Hintergrundfarbe. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddFillColorFilterWithInt32BackgroundTypeCellsColorCDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten mit verschiedenen Füllfarben hinzufügen
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A3"].PutValue("Data2");
            cells["A4"].PutValue("Data3");
            
            // Verschiedene Füllfarben anwenden
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

            // Automatischen Filter erstellen
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Zellenfarbe für Filterung erstellen
            CellsColor filterColor = workbook.CreateCellsColor();
            filterColor.Color = Color.Red;
            
            // Füllfarbfilter anwenden
            filter.AddFillColorFilter(0, BackgroundType.Solid, filterColor, filterColor);
            filter.Refresh();
            
            // Speichere die Arbeitsmappe
            workbook.Save("AutoFilterFillColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [BackgroundType](../../backgroundtype/)
* class [CellsColor](../../cellscolor/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



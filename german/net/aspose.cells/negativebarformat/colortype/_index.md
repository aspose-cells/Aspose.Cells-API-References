---
title: "NegativeBarFormat.ColorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NegativeBarFormat property. Gibt an, ob dieselbe Füllfarbe wie bei positiven Datenbalken verwendet werden soll, und ermöglicht das Festlegen"
type: docs
url: /de/net/aspose.cells/negativebarformat/colortype/
---
## NegativeBarFormat.ColorType property

Liest oder setzt, ob die gleiche Füllfarbe wie bei positiven Datenbalken verwendet werden soll.

```csharp
public DataBarNegativeColorType ColorType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class NegativeBarFormatPropertyColorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-15);
            sheet.Cells["F4"].PutValue(25);
            sheet.Cells["G3"].PutValue(-5);
            sheet.Cells["G4"].PutValue(15);

            // Bereich für bedingte Formatierung erstellen
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.StartColumn = 4;
            area.EndRow = 3;
            area.EndColumn = 6;

            // Bedingte Formatierung für Datenbalken hinzufügen
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            conds.AddArea(area);
            
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Datenbalken-Eigenschaften festlegen
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            
            // Negatives Balkenformat konfigurieren
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Speichere die Arbeitsmappe
            workbook.Save("NegativeBarFormatDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Demo completed. File saved with negative bar formatting.");
        }
    }
}
```

### Siehe auch

* enum [DataBarNegativeColorType](../../databarnegativecolortype/)
* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



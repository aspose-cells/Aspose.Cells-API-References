---
title: "NegativeBarFormat.BorderColorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "NegativeBarFormat property. Gibt an, ob dieselbe Rahmenfarbe wie bei positiven Datenbalken verwendet werden soll"
type: docs
url: /de/net/aspose.cells/negativebarformat/bordercolortype/
---
## NegativeBarFormat.BorderColorType property

Gibt an, ob die gleiche Rahmenfarbe wie bei positiven Datenbalken verwendet werden soll.

```csharp
public DataBarNegativeColorType BorderColorType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class NegativeBarFormatPropertyBorderColorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-50);
            sheet.Cells["G4"].PutValue(60);

            // Bedingte Formatierung für Datenbalken hinzufügen
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];

            // Datenbalken einrichten
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;

            // Datenbalkenrahmen festlegen
            cond.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            cond.DataBar.BarBorder.Color = Color.Plum;

            // Negatives Balkenformat festlegen
            cond.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.Color = Color.White;
            
            // BorderColorType-Eigenschaft demonstrieren
            cond.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            cond.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Speichere die Arbeitsmappe
            workbook.Save("NegativeBarFormatBorderColorTypeDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Demo completed. File saved.");
        }
    }
}
```

### Siehe auch

* enum [DataBarNegativeColorType](../../databarnegativecolortype/)
* class [NegativeBarFormat](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



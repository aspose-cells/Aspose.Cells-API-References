---
title: "DataBar.NegativeBarFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataBar-Eigenschaft. Gibt das NegativeBarFormat-Objekt zurück, das mit einer DataBar-Bedingten-Formatierungsregel verknüpft ist"
type: docs
url: /de/net/aspose.cells/databar/negativebarformat/
---
## DataBar.NegativeBarFormat property

Liest das NegativeBarFormat-Objekt, das mit einer bedingten Formatierungsregel für Datenbalken verknüpft ist.

```csharp
public NegativeBarFormat NegativeBarFormat { get; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyNegativeBarFormatDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten mit negativen Werten hinzufügen
            sheet.Cells["E3"].PutValue(-10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(-30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-50);
            sheet.Cells["G4"].PutValue(60);

            // Bedingte Formatierung für Datenbalken hinzufügen
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = sheet.ConditionalFormattings[formatIndex];
            int index = conditions.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditions[index];

            // Datenbalken-Eigenschaften festlegen
            condition.DataBar.Color = Color.Orange;
            condition.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            condition.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            condition.DataBar.ShowValue = false;

            // Rahmen-Eigenschaften festlegen
            condition.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            condition.DataBar.BarBorder.Color = Color.Plum;

            // Fülltyp festlegen
            condition.DataBar.BarFillType = DataBarFillType.Gradient;

            // Achsen-Eigenschaften festlegen
            condition.DataBar.AxisColor = Color.Red;
            condition.DataBar.AxisPosition = DataBarAxisPosition.Automatic;

            // Negatives Balkenformat konfigurieren
            condition.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.Color = Color.White;
            condition.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Speichere die Arbeitsmappe
            workbook.Save("DataBarNegativeFormatDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [NegativeBarFormat](../../negativebarformat/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "ColorScale.MinColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ColorScale-Eigenschaft. Abrufen oder Festlegen der Verlaufsfarbe für den Minimalwert im Bereich"
type: docs
url: /de/net/aspose.cells/colorscale/mincolor/
---
## ColorScale.MinColor property

Abrufen oder Festlegen der Verlaufsfarbe für den Minimalwert im Bereich.

```csharp
public Color MinColor { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMinColorDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Bedingte Formatierung hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Erstelle ein CellArea-Objekt anstelle einer Zeichenkette zu verwenden
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcs.AddArea(area);

            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Farbskala konfigurieren
            ColorScale colorScale = fc.ColorScale;
            colorScale.MinColor = Color.Green;
            colorScale.MidColor = Color.Yellow;
            colorScale.MaxColor = Color.Red;

            // Werttypen festlegen
            colorScale.MinCfvo.Type = FormatConditionValueType.Min;
            colorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            colorScale.MidCfvo.Value = 50;
            colorScale.MaxCfvo.Type = FormatConditionValueType.Max;

            // Speichere die Arbeitsmappe
            workbook.Save("ColorScaleMinColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "ColorScale.MaxColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ColorScale-Eigenschaft. Abrufen oder Festlegen der Farbverlauffarbe für den Maximalwert im Bereich"
type: docs
url: /de/net/aspose.cells/colorscale/maxcolor/
---
## ColorScale.MaxColor property

Lese oder setze die Verlaufsfarbe für den Maximalwert im Bereich.

```csharp
public Color MaxColor { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMaxColorDemo
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
            worksheet.Cells["A5"].PutValue(50);

            // Bedingte Formatierung hinzufügen
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Erstelle ein CellArea-Objekt anstelle einer Zeichenkette zu verwenden
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Farbskalenbedingung hinzufügen
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];
            ColorScale colorScale = fc.ColorScale;

            // Farbskala konfigurieren
            colorScale.Is3ColorScale = false; // Use 2-color scale for simplicity
            colorScale.MinColor = Color.Green;
            colorScale.MaxColor = Color.Red; // Demonstrating MaxColor property

            // Wertobjekte festlegen
            colorScale.MinCfvo.Type = FormatConditionValueType.Min;
            colorScale.MaxCfvo.Type = FormatConditionValueType.Max;

            // Speichere die Arbeitsmappe
            workbook.Save("ColorScaleMaxColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



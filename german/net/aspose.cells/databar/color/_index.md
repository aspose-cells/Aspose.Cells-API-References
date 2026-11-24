---
title: "DataBar.Color"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataBar-Eigenschaft. Gibt die Farbe dieses Datenbalkens zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/databar/color/
---
## DataBar.Color property

Lese oder setze die Farbe dieses Datenbalkens.

```csharp
public Color Color { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen Zellbereich
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.StartColumn = 4;
            area.EndRow = 3;
            area.EndColumn = 6;

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["E3"].PutValue(10);
            worksheet.Cells["F3"].PutValue(20);
            worksheet.Cells["G3"].PutValue(30);
            worksheet.Cells["E4"].PutValue(15);
            worksheet.Cells["F4"].PutValue(25);
            worksheet.Cells["G4"].PutValue(35);

            // Bedingte Formatierung mit Datenbalken hinzufügen
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[formatIndex];
            int index = conditions.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditions[index];

            // Datenbalken-Eigenschaften einschließlich Farbe festlegen
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

            // Negative Balken-Eigenschaften festlegen
            condition.DataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.Color = Color.White;
            condition.DataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            condition.DataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Formatierung auf den Bereich anwenden
            conditions.AddArea(area);

            // Speichere die Arbeitsmappe
            workbook.Save("DataBarPropertyColorDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBarPropertyColorDemo executed successfully.");
        }
    }
}
```

### Siehe auch

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



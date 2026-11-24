---
title: "ColorScale.MinCfvo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ColorScale-Eigenschaft. Abrufen oder Festlegen dieses Minimalwertobjekts der ColorScales. Null oder ein CFValueObject mit dem Typ FormatConditionValueType.Max kann nicht gesetzt werden."
type: docs
url: /de/net/aspose.cells/colorscale/mincfvo/
---
## ColorScale.MinCfvo property

Abrufen oder Festlegen des Minimalwertobjekts dieses ColorScale. Null oder CFValueObject mit dem Typ FormatConditionValueType.Max kann nicht dafür festgelegt werden.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMinCfvoDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Erstelle eine bedingte Formatierung mit Farbskala
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Farbskala hinzufügen
            int csIndex = fcc.AddCondition(FormatConditionType.ColorScale);
            ColorScale cs = fcc[csIndex].ColorScale;

            // MinCfvo-Eigenschaften festlegen
            cs.MinCfvo.Type = FormatConditionValueType.Min;
            cs.MinCfvo.Value = "0";
            cs.MinColor = System.Drawing.Color.Red;

            // MidCfvo-Eigenschaften festlegen
            cs.MidCfvo.Type = FormatConditionValueType.Percentile;
            cs.MidCfvo.Value = "50";
            cs.MidColor = System.Drawing.Color.Yellow;

            // MaxCfvo-Eigenschaften festlegen
            cs.MaxCfvo.Type = FormatConditionValueType.Max;
            cs.MaxCfvo.Value = "0";
            cs.MaxColor = System.Drawing.Color.Green;

            // Speichere die Arbeitsmappe
            workbook.Save("ColorScaleMinCfvoDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



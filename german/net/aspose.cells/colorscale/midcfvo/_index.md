---
title: "ColorScale.MidCfvo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ColorScale-Eigenschaft. Abrufen oder Festlegen dieses Mittelwertobjekts der ColorScales. Ein CFValueObject mit dem Typ FormatConditionValueType.Max oder FormatConditionValueType.Min kann nicht gesetzt werden."
type: docs
url: /de/net/aspose.cells/colorscale/midcfvo/
---
## ColorScale.MidCfvo property

Abrufen oder Festlegen des Midwertobjekts dieses ColorScale. CFValueObject mit dem Typ FormatConditionValueType.Max oder FormatConditionValueType.Min kann nicht dafür festgelegt werden.

```csharp
public ConditionalFormattingValue MidCfvo { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMidCfvoDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i * 10);
            }

            // Füge eine bedingte Formatierung mit Farbskala hinzu
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            int conditionIndex = fcc.AddCondition(FormatConditionType.ColorScale);
            
            // Setze den Mittelwert für die Farbskala
            ColorScale colorScale = fcc[conditionIndex].ColorScale;
            colorScale.MidCfvo.Type = FormatConditionValueType.Number;
            colorScale.MidCfvo.Value = 50;

            // Speichere die Arbeitsmappe
            workbook.Save("ColorScalePropertyMidCfvoDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



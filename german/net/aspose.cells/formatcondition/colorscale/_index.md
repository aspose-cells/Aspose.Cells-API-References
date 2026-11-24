---
title: "FormatCondition.ColorScale"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FormatCondition-Eigenschaft. Rufen Sie die ColorScale-Instanz der bedingten Formatierung ab. Die Standardinstanz ist ein grün-gelb-rot 3ColorScale. Nur gültig für den Typ ColorScale."
type: docs
url: /de/net/aspose.cells/formatcondition/colorscale/
---
## FormatCondition.ColorScale property

Rufen Sie die "ColorScale"-Instanz der bedingten Formatierung ab. Die Standardinstanz ist ein "grün-gelb-rot" 3ColorScale. Gültig nur für Typ = ColorScale.

```csharp
public ColorScale ColorScale { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyColorScaleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Füge eine bedingte Formatierung mit Farbskala hinzu
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Legen Sie den Bereich für die bedingte Formatierung fest
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Legen Sie die ColorScale-Eigenschaften fest
            fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[0];
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Green;

            // Speichere die Arbeitsmappe
            workbook.Save("ColorScaleExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [ColorScale](../../colorscale/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



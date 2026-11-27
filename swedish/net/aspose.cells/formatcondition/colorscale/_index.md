---
title: "FormatCondition.ColorScale"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormatCondition-egenskap. Hämta den villkorliga formateringens ColorScale-instans. Standardinstansen är en gröngulröd 3ColorScale. Giltig endast för typen ColorScale"
type: docs
url: /sv/net/aspose.cells/formatcondition/colorscale/
---
## FormatCondition.ColorScale property

Hämta den villkorliga formateringens "ColorScale"-instans. Standardinstansen är en "grön-gul-röd" 3ColorScale. Giltig endast för typ = ColorScale.

```csharp
public ColorScale ColorScale { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Lägg till en färgskala för villkorlig formatering
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Ange området för villkorsformateringen
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Ställ in färgskalans egenskaper
            fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[0];
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Green;

            // Spara arbetsboken
            workbook.Save("ColorScaleExample.xlsx");
        }
    }
}
```

### Se även

* class [ColorScale](../../colorscale/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



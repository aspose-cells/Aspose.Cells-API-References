---
title: "ColorScale.MaxCfvo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ColorScale. Obtenga o establezca este objeto de valor máximo de ColorScales. No se puede establecer null o CFValueObject con tipo FormatConditionValueType.Min en él"
type: docs
url: /es/net/aspose.cells/colorscale/maxcfvo/
---
## ColorScale.MaxCfvo property

Obtener o establecer el objeto de valor máximo de este ColorScale. No se puede establecer null o CFValueObject con tipo FormatConditionValueType.Min en él.

```csharp
public ConditionalFormattingValue MaxCfvo { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMaxCfvoDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            ws.Cells["A1"].PutValue(1);
            ws.Cells["A2"].PutValue(2);
            ws.Cells["A3"].PutValue(3);
            ws.Cells["A4"].PutValue(4);
            ws.Cells["A5"].PutValue(5);

            int idx = ws.ConditionalFormattings.Add();
            FormatConditionCollection fcc = ws.ConditionalFormattings[idx];
            fcc.AddArea(CellArea.CreateCellArea("A1", "A5"));

            idx = fcc.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcc[idx];
            
            fc.ColorScale.Is3ColorScale = false;
            
            // Demostrar el uso de la propiedad MaxCfvo
            fc.ColorScale.MaxCfvo.IsGTE = true;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Yellow;
            
            fc.ColorScale.MinCfvo.IsGTE = true;
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;

            workbook.Save("ColorScaleMaxCfvoDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "ColorScale.MidCfvo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ColorScale. Obtenga o establezca este objeto de valor medio de ColorScales. No se puede establecer CFValueObject con tipo FormatConditionValueType.Max o FormatConditionValueType.Min en él"
type: docs
url: /es/net/aspose.cells/colorscale/midcfvo/
---
## ColorScale.MidCfvo property

Obtener o establecer el objeto de valor medio de este ColorScale. No se puede establecer CFValueObject con tipo FormatConditionValueType.Max o FormatConditionValueType.Min en él.

```csharp
public ConditionalFormattingValue MidCfvo { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMidCfvoDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i * 10);
            }

            // Agregar un formato condicional de escala de color
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            int conditionIndex = fcc.AddCondition(FormatConditionType.ColorScale);
            
            // Establecer el valor del punto medio para la escala de color
            ColorScale colorScale = fcc[conditionIndex].ColorScale;
            colorScale.MidCfvo.Type = FormatConditionValueType.Number;
            colorScale.MidCfvo.Value = 50;

            // Guarda el libro de trabajo
            workbook.Save("ColorScalePropertyMidCfvoDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



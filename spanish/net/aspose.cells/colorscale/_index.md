---
title: "Clase ColorScale"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ColorScale. Describe la regla de formato condicional ColorScale. Esta regla de formato condicional crea una escala de colores graduada en las celdas"
type: docs
url: /es/net/aspose.cells/colorscale/
---
## ColorScale class

Describe la regla de formato condicional ColorScale. Esta regla de formato condicional crea una escala de colores graduada en las celdas.

```csharp
public class ColorScale
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Is3ColorScale](../../aspose.cells/colorscale/is3colorscale/) { get; set; } | Indica si el formato condicional es una escala de 3 colores. |
| [MaxCfvo](../../aspose.cells/colorscale/maxcfvo/) { get; } | Obtener o establecer el objeto de valor máximo de este ColorScale. No se puede establecer null o CFValueObject con tipo FormatConditionValueType.Min en él. |
| [MaxColor](../../aspose.cells/colorscale/maxcolor/) { get; set; } | Obtener o establecer el color degradado para el valor máximo en el rango. |
| [MidCfvo](../../aspose.cells/colorscale/midcfvo/) { get; } | Obtener o establecer el objeto de valor medio de este ColorScale. No se puede establecer CFValueObject con tipo FormatConditionValueType.Max o FormatConditionValueType.Min en él. |
| [MidColor](../../aspose.cells/colorscale/midcolor/) { get; set; } | Obtener o establecer el color degradado para el valor medio en el rango. |
| [MinCfvo](../../aspose.cells/colorscale/mincfvo/) { get; } | Obtener o establecer el objeto de valor mínimo de este ColorScale. No se puede establecer null o CFValueObject con tipo FormatConditionValueType.Max en él. |
| [MinColor](../../aspose.cells/colorscale/mincolor/) { get; set; } | Obtener o establecer el color degradado para el valor mínimo en el rango. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColorScaleDemo
    {
        public static void ColorScaleExample()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo a la hoja de cálculo
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i * j);
                }
            }

            // Agregar una regla de formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 9, StartColumn = 0, EndColumn = 9 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Acceder al objeto ColorScale
            ColorScale colorScale = fc.ColorScale;

            // Establecer propiedades para el ColorScale
            colorScale.Is3ColorScale = true;
            colorScale.MinColor = Color.Green;
            colorScale.MidColor = Color.Yellow;
            colorScale.MaxColor = Color.Red;

            // Establecer los objetos de valor min, medio y max
            ConditionalFormattingValue minCfvo = colorScale.MinCfvo;
            minCfvo.Type = FormatConditionValueType.Min;
            minCfvo.Value = null;

            ConditionalFormattingValue midCfvo = colorScale.MidCfvo;
            midCfvo.Type = FormatConditionValueType.Percentile;
            midCfvo.Value = 50;

            ConditionalFormattingValue maxCfvo = colorScale.MaxCfvo;
            maxCfvo.Type = FormatConditionValueType.Max;
            maxCfvo.Value = null;

            // Guarda el libro de trabajo
            workbook.Save("ColorScaleExample.xlsx");
            workbook.Save("ColorScaleExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



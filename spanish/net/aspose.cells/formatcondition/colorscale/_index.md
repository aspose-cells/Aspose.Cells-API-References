---
title: "FormatCondition.ColorScale"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormatCondition. Obtén la instancia ColorScale del formato condicional. La instancia predeterminada es un greenyellowred 3ColorScale. Válido solo para el tipo ColorScale"
type: docs
url: /es/net/aspose.cells/formatcondition/colorscale/
---
## FormatCondition.ColorScale property

Obtenga la instancia "ColorScale" del formato condicional. La instancia predeterminada es una "green-yellow-red" 3ColorScale. Válido solo para type = ColorScale.

```csharp
public ColorScale ColorScale { get; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Agregar un formato condicional de escala de color
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Establecer el rango para el formato condicional
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Establecer las propiedades de la escala de colores
            fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[0];
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Green;

            // Guarda el libro de trabajo
            workbook.Save("ColorScaleExample.xlsx");
        }
    }
}
```

### Ver también

* class [ColorScale](../../colorscale/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



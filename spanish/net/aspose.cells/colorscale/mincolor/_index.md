---
title: "ColorScale.MinColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ColorScale. Obtenga o establezca el color degradado para el valor mínimo en el rango"
type: docs
url: /es/net/aspose.cells/colorscale/mincolor/
---
## ColorScale.MinColor property

Obtener o establecer el color degradado para el valor mínimo en el rango.

```csharp
public Color MinColor { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMinColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Cree el objeto CellArea en lugar de usar una cadena
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcs.AddArea(area);

            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // Configurar escala de colores
            ColorScale colorScale = fc.ColorScale;
            colorScale.MinColor = Color.Green;
            colorScale.MidColor = Color.Yellow;
            colorScale.MaxColor = Color.Red;

            // Establecer tipos de valor
            colorScale.MinCfvo.Type = FormatConditionValueType.Min;
            colorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            colorScale.MidCfvo.Value = 50;
            colorScale.MaxCfvo.Type = FormatConditionValueType.Max;

            // Guarda el libro de trabajo
            workbook.Save("ColorScaleMinColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



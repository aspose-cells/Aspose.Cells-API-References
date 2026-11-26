---
title: "ColorScale.MinCfvo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ColorScale. Obtenga o establezca este objeto de valor mínimo de ColorScales. No se puede establecer null o CFValueObject con tipo FormatConditionValueType.Max en él"
type: docs
url: /es/net/aspose.cells/colorscale/mincfvo/
---
## ColorScale.MinCfvo property

Obtener o establecer el objeto de valor mínimo de este ColorScale. No se puede establecer null o CFValueObject con tipo FormatConditionValueType.Max en él.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Crear un formato condicional de escala de color
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Agregar escala de color
            int csIndex = fcc.AddCondition(FormatConditionType.ColorScale);
            ColorScale cs = fcc[csIndex].ColorScale;

            // Establecer propiedades de MinCfvo
            cs.MinCfvo.Type = FormatConditionValueType.Min;
            cs.MinCfvo.Value = "0";
            cs.MinColor = System.Drawing.Color.Red;

            // Establecer propiedades de MidCfvo
            cs.MidCfvo.Type = FormatConditionValueType.Percentile;
            cs.MidCfvo.Value = "50";
            cs.MidColor = System.Drawing.Color.Yellow;

            // Establecer propiedades de MaxCfvo
            cs.MaxCfvo.Type = FormatConditionValueType.Max;
            cs.MaxCfvo.Value = "0";
            cs.MaxColor = System.Drawing.Color.Green;

            // Guarda el libro de trabajo
            workbook.Save("ColorScaleMinCfvoDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



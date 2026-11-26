---
title: "ColorScale.MaxColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ColorScale. Obtenga o establezca el color degradado para el valor máximo en el rango"
type: docs
url: /es/net/aspose.cells/colorscale/maxcolor/
---
## ColorScale.MaxColor property

Obtener o establecer el color degradado para el valor máximo en el rango.

```csharp
public Color MaxColor { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColorScalePropertyMaxColorDemo
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
            worksheet.Cells["A5"].PutValue(50);

            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Cree el objeto CellArea en lugar de usar una cadena
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // Agregar condición de escala de colores
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];
            ColorScale colorScale = fc.ColorScale;

            // Configurar escala de colores
            colorScale.Is3ColorScale = false; // Use 2-color scale for simplicity
            colorScale.MinColor = Color.Green;
            colorScale.MaxColor = Color.Red; // Demonstrating MaxColor property

            // Establecer objetos de valor
            colorScale.MinCfvo.Type = FormatConditionValueType.Min;
            colorScale.MaxCfvo.Type = FormatConditionValueType.Max;

            // Guarda el libro de trabajo
            workbook.Save("ColorScaleMaxColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ColorScale](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



---
title: "Clase NegativeBarFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.NegativeBarFormat. Representa la configuración de color de las barras de datos para valores negativos que se definen mediante una regla de formato condicional de barra de datos"
type: docs
url: /es/net/aspose.cells/negativebarformat/
---
## NegativeBarFormat class

Representa la configuración de color de las barras de datos para valores negativos que se definen mediante una regla de formato condicional de barra de datos.

```csharp
public class NegativeBarFormat
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BorderColor](../../aspose.cells/negativebarformat/bordercolor/) { get; set; } | Obtiene o establece un objeto FormatColor que puede usar para especificar el color del borde de las barras de datos negativas. |
| [BorderColorType](../../aspose.cells/negativebarformat/bordercolortype/) { get; set; } | Indica si se debe usar el mismo color de borde que las barras de datos positivas. |
| [Color](../../aspose.cells/negativebarformat/color/) { get; set; } | Obtiene o establece un objeto FormatColor que puede usar para especificar el color de relleno de las barras de datos negativas. |
| [ColorType](../../aspose.cells/negativebarformat/colortype/) { get; set; } | Obtiene o establece si se debe usar el mismo color de relleno que las barras de datos positivas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class NegativeBarFormatDemo
    {
        public static void NegativeBarFormatExample()
        {
            // Instanciar un objeto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega un formato condicional vacío
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Establece el rango de formato condicional
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Agrega una condición para DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Obtén DataBar y establece sus propiedades
            DataBar dataBar = fc.DataBar;
            dataBar.Color = Color.Orange;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;

            // Configura las propiedades de NegativeBarFormat
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = Color.White;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = Color.Yellow;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;

            // Introduce algunos valores en las celdas
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);

            // Guarda el libro de trabajo
            workbook.Save("NegativeBarFormatExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



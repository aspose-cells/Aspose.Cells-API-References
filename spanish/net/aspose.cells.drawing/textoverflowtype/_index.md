---
title: "Enum TextOverflowType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.TextOverflowType enum. Representa la forma en que el texto se desborda vertical u horizontalmente."
type: docs
url: /es/net/aspose.cells.drawing/textoverflowtype/
---
## TextOverflowType enumeration

Representa la forma en que el texto desborda vertical u horizontalmente.

```csharp
public enum TextOverflowType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Clip | `0` | Preste atención a las barreras superior e inferior. No proporcione indicación de que hay texto que no es visible. |
| Ellipsis | `1` | Preste atención a las barreras superior e inferior. Use una elipsis para indicar que hay texto que no es visible. Solo para desbordamiento vertical. |
| Overflow | `2` | Desborde el texto y no preste atención a las barreras superior e inferior. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DrawingClassTextOverflowTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Agregar un cuadro de texto al gráfico
            TextBox textBox = chart.Shapes.AddTextBoxInChart(10, 10, 200, 50);

            // Establecer propiedades del cuadro de texto
            textBox.TextBody.TextAlignment.AutoSize = false;
            textBox.Text = "This is a long text that will demonstrate text overflow handling";
            
            // Establecer tipo de desbordamiento de texto
            textBox.TextVerticalOverflow = TextOverflowType.Clip;

            // Guarda el libro de trabajo
            workbook.Save("TextOverflowTypeDemo_out.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



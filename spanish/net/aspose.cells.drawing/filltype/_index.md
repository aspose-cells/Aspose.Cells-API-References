---
title: "Enum FillType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.FillType enum. Tipo de formato de relleno"
type: docs
url: /es/net/aspose.cells.drawing/filltype/
---
## FillType enumeration

Tipo de formato de relleno.

```csharp
public enum FillType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Automatic | `0` | Representa el tipo de formato automático. |
| None | `1` | Representa el tipo de formato ninguno. |
| Solid | `2` | Formato de relleno sólido. |
| Gradient | `3` | Formato de relleno degradado. |
| Texture | `4` | Formato de relleno de textura (incluye relleno de imagen). |
| Pattern | `5` | Formato de relleno de patrón. |
| Group | `6` | Heredar las propiedades de relleno del grupo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 150);
            
            // Establecer el tipo de relleno de degradado
            rectangle.Fill.FillType = FillType.Gradient;
            rectangle.Fill.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);

            // Agregar un cuadro de texto
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 10, 10, 100, 150);
            textBox.Text = "Gradient Fill Example";
            
            // Establecer el tipo de relleno degradado para el cuadro de texto
            textBox.Fill.FillType = FillType.Gradient;
            textBox.Fill.SetTwoColorGradient(Color.LightGreen, Color.DarkGreen, GradientStyleType.Vertical, 1);

            // Guarda el libro de trabajo
            workbook.Save("FillTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



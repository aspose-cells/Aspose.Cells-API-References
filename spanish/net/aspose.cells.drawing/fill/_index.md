---
title: "Clase Fill"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Fill. Representa el formato de relleno de la forma"
type: docs
url: /es/net/aspose.cells.drawing/fill/
---
## Fill class

Representa el formato de relleno de la forma.

```csharp
public abstract class Fill
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | / |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Obtiene el código hash. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassFillDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 150);
            // Establecer el tipo de relleno a sólido y modificar el color
            rectangle.Fill.FillType = FillType.Solid;
            rectangle.Fill.SolidFill.Color = Color.LightBlue;

            Shape oval = worksheet.Shapes.AddOval(2, 0, 0, 0, 100, 150);
            // Usar el método de relleno degradado directamente en FillFormat
            oval.Fill.SetTwoColorGradient(Color.DarkBlue, Color.SkyBlue, GradientStyleType.Vertical, 0);

            workbook.Save("DrawingClassFillDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



---
title: "Clase MsoFillFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.MsoFillFormat. Representa el formato de relleno para una shape"
type: docs
url: /es/net/aspose.cells.drawing/msofillformat/
---
## MsoFillFormat class

Representa el formato de relleno para una forma.

```csharp
public class MsoFillFormat
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msofillformat/backcolor/) { get; set; } | Obtiene y establece el color de fondo del archivo. |
| [ForeColor](../../aspose.cells.drawing/msofillformat/forecolor/) { get; set; } | Obtiene y establece el color de primer plano del relleno. |
| [ImageData](../../aspose.cells.drawing/msofillformat/imagedata/) { get; set; } | Obtiene y establece los datos de relleno de textura y de imagen. |
| [IsVisible](../../aspose.cells.drawing/msofillformat/isvisible/) { get; set; } | Indica si hay relleno. |
| [Texture](../../aspose.cells.drawing/msofillformat/texture/) { get; } | Obtiene el tipo de relleno de textura. |
| [Transparency](../../aspose.cells.drawing/msofillformat/transparency/) { get; set; } | Devuelve o establece el grado de transparencia del relleno especificado como un valor de 0.0 (opaco) a 1.0 (claro). |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetOneColorGradient](../../aspose.cells.drawing/msofillformat/setonecolorgradient/)(Color, double, GradientStyleType, int) | Establece el relleno especificado a un degradado de un solo color. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatDemo
    {
        public static void MsoFillFormatExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de arco a la hoja de cálculo
            Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Acceder al formato de relleno de la shape
            MsoFillFormat fillFormat = arcShape.FillFormat;

            // Establecer el color frontal del relleno
            fillFormat.ForeColor = Color.Blue;

            // Establecer el color de fondo del relleno
            fillFormat.BackColor = Color.LightBlue;

            // Establecer la transparencia
            fillFormat.Transparency = 0.5;

            // Verificar si el relleno es visible
            bool isVisible = fillFormat.IsVisible;
            Console.WriteLine("Is Fill Visible: " + isVisible);

            // Establecer un relleno degradado de un solo color
            fillFormat.SetOneColorGradient(Color.Green, 0.3, GradientStyleType.Horizontal, 1);

            // Guarda el libro de trabajo
            workbook.Save("MsoFillFormatExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



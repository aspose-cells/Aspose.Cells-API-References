---
title: "ShapePath.HeightPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapePath. Obtiene la altura de esta ruta en unidades de píxeles"
type: docs
url: /es/net/aspose.cells.drawing/shapepath/heightpixel/
---
## ShapePath.HeightPixel property

Obtiene la altura de esta ruta en unidades de píxeles.

```csharp
public int HeightPixel { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyHeightPixelDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crear una nueva ruta de forma
                ShapePath shapePath = new ShapePath();

                // Crear una ruta rectangular simple
                shapePath.MoveTo(10, 10);
                shapePath.LineTo(100, 10);
                shapePath.LineTo(100, 50);
                shapePath.LineTo(10, 50);
                shapePath.Close();

                // Mostrar el valor actual de HeightPixel
                Console.WriteLine("Initial HeightPixel value: " + shapePath.HeightPixel);

                // Establecer un nuevo valor de altura
                shapePath.HeightPixel = 200;
                Console.WriteLine("Updated HeightPixel value: " + shapePath.HeightPixel);

                // Agregar la forma a la hoja de cálculo
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                // Guarda el libro de trabajo
                workbook.Save("HeightPixelDemo.xlsx");
                Console.WriteLine("HeightPixel property demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



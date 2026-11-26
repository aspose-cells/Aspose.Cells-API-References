---
title: "ShapePath.WidthPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapePath. Obtiene el ancho de esta ruta en unidades de píxeles"
type: docs
url: /es/net/aspose.cells.drawing/shapepath/widthpixel/
---
## ShapePath.WidthPixel property

Obtiene el ancho de esta ruta en unidades de píxeles.

```csharp
public int WidthPixel { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyWidthPixelDemo
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

                // Mostrar el valor inicial de WidthPixel
                Console.WriteLine("Initial WidthPixel value: " + shapePath.WidthPixel);

                // Establecer un nuevo valor de ancho
                shapePath.WidthPixel = 300;
                Console.WriteLine("Updated WidthPixel value: " + shapePath.WidthPixel);

                // Agregar la forma a la hoja de cálculo
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, shapePath.WidthPixel, 200, new ShapePath[] { shapePath });

                // Guarda el libro de trabajo
                workbook.Save("WidthPixelDemo.xlsx");
                Console.WriteLine("WidthPixel property demonstrated successfully.");
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



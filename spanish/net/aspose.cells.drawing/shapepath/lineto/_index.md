---
title: "ShapePath.LineTo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapePath. Añade un segmento de línea a la figura actual. El punto de inicio es el punto final de la figura actual. Unidad Pixel"
type: docs
url: /es/net/aspose.cells.drawing/shapepath/lineto/
---
## ShapePath.LineTo method

Añade un segmento de línea a la figura actual. El punto de inicio es el punto final de la figura actual. Unidad: Pixel.

```csharp
public void LineTo(float x, float y)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| x | Single | La coordenada x del punto final del segmento de línea (Unidad: Pixel). |
| y | Single | La coordenada y del punto final del segmento de línea (Unidad: Pixel). |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodLineToWithSingleSingleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //Crear una nueva ruta de forma
                ShapePath shapePath = new ShapePath();

                // Mover al punto de inicio
                shapePath.MoveTo(10, 10);
                
                // Llamar al método LineTo con parámetros (Single, Single)
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                //agregar forma libre
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("LineTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("ShapePathMethodLineToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



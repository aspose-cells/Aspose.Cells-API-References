---
title: "ShapePath.MoveTo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapePath. Inicia una nueva figura desde el punto especificado sin cerrar la figura actual. Todos los puntos posteriores añadidos a la ruta se añaden a esta nueva figura. Unidad píxel"
type: docs
url: /es/net/aspose.cells.drawing/shapepath/moveto/
---
## ShapePath.MoveTo method

Inicia una nueva figura desde el punto especificado sin cerrar la figura actual. Todos los puntos posteriores añadidos a la ruta se añaden a esta nueva figura. Unidad: Pixel.

```csharp
public void MoveTo(float x, float y)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| x | Single | La coordenada x del punto de inicio de la figura (Unidad: píxel). |
| y | Single | La coordenada y del punto de inicio de la figura (Unidad: píxel). |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodMoveToWithSingleSingleDemo
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

                Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
           
            
            // Guardar el resultado
            workbook.Save("ShapePathMethodMoveToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



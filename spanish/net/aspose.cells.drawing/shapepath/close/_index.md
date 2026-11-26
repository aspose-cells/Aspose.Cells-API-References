---
title: "ShapePath.Close"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapePath. Cierra la figura actual e inicia una nueva figura. Si la figura actual contiene una secuencia de líneas y curvas conectadas, el método cierra el bucle conectando una línea desde el punto final hasta el punto de inicio."
type: docs
url: /es/net/aspose.cells.drawing/shapepath/close/
---
## ShapePath.Close method

Cierra la figura actual e inicia una nueva figura. Si la figura actual contiene una secuencia de líneas y curvas conectadas, el método cierra el bucle conectando una línea desde el punto final hasta el punto de inicio.

```csharp
public void Close()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCloseDemo
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
                shapePath.MoveTo(60, 45);
                shapePath.ArcTo(25, 25, 0, 270);

                // Cerrar la ruta 
                shapePath.Close();

                shapePath.MoveTo(60, 20);
                shapePath.LineTo(110, 70);
                shapePath.LineTo(125, 155.5f);
                shapePath.ArcTo(35.5f, 35.5f, 0, 270);

                // Cerrar la ruta 
                shapePath.Close();

                //agregar forma libre
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("Close method called successfully to complete the shape path");
                
                // Guarda el libro de trabajo
                workbook.Save("ShapePathMethodCloseDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Close method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



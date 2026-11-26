---
title: "Clase DrawObjectEventHandler"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Rendering.DrawObjectEventHandler. Interfaz para obtener DrawObject y Bound al renderizar"
type: docs
url: /es/net/aspose.cells.rendering/drawobjecteventhandler/
---
## DrawObjectEventHandler class

Interfaz para obtener DrawObject y Bound durante el renderizado.

```csharp
public abstract class DrawObjectEventHandler
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [Draw](../../aspose.cells.rendering/drawobjecteventhandler/draw/)(DrawObject, float, float, float, float) | Implemente esta interfaz para obtener DrawObject y Bound al renderizar. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassDrawObjectEventHandlerDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B2"].PutValue(12345);
            worksheet.Shapes.AddRectangle(5, 5, 50, 100, 200, 300); // Added missing parameter

            // Crear opciones de guardado PDF con un controlador de renderizado personalizado
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectHandler();

            // Guardar el libro de trabajo en PDF con personalización del renderizado
            workbook.Save("DrawObjectEventHandlerDemo.pdf", saveOptions);
        }
    }

    public class CustomDrawObjectHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Demostrar el manejo de diferentes tipos de objetos de renderizado
            switch (drawObject.Type)
            {
                case DrawObjectEnum.Cell:
                    Console.WriteLine($"Rendering cell at ({x}, {y})");
                    break;
                    
                case DrawObjectEnum.Image:
                    Console.WriteLine($"Rendering image at ({x}, {y})");
                    break;
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)



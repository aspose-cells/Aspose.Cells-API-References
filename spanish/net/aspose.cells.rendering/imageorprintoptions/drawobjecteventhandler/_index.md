---
title: "ImageOrPrintOptions.DrawObjectEventHandler"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Implementa esta interfaz para obtener DrawObject y Bound al renderizar"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/
---
## ImageOrPrintOptions.DrawObjectEventHandler property

Implemente esta interfaz para obtener DrawObject y Bound al renderizar.

```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyDrawObjectEventHandlerDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);

            // Crear un controlador de eventos DrawObject personalizado
            var drawHandler = new CustomDrawObjectEventHandler();

            // Establecer opciones de imagen con el manejador de eventos
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.DrawObjectEventHandler = drawHandler;

            // Renderizar la hoja de cálculo para activar los eventos
            SheetRender render = new SheetRender(worksheet, options);
            for (int pageIndex = 0; pageIndex < render.PageCount; pageIndex++)
            {
                using (MemoryStream stream = new MemoryStream())
                {
                    render.ToImage(pageIndex, stream);
                }
            }
        }
    }

    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Ejemplo: Imprimir información sobre el objeto dibujado
            Console.WriteLine($"Drawing {drawObject.Type} at ({x},{y}) with size {width}x{height}");
        }
    }
}
```

### Ver también

* class [DrawObjectEventHandler](../../drawobjecteventhandler/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



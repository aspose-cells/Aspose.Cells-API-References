---
title: "PaginatedSaveOptions.DrawObjectEventHandler"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Implementa esta interfaz para obtener DrawObject y Bound al renderizar"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/drawobjecteventhandler/
---
## PaginatedSaveOptions.DrawObjectEventHandler property

Implemente esta interfaz para obtener DrawObject y Bound al renderizar.

```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PaginatedSaveOptionsPropertyDrawObjectEventHandlerDemo
    {
        private class CustomDrawObjectEventHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine($"Position: X={x}, Y={y}, Width={width}, Height={height}");
            }
        }

        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de muestra y formas
            worksheet.Cells["A1"].PutValue("Test DrawObjectEventHandler");
            worksheet.Cells["A2"].PutValue("This will demonstrate the event handler during rendering");
            
            // Crear una instancia de PaginatedSaveOptions
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Mostrar el valor actual de la propiedad (debe ser null inicialmente)
            Console.WriteLine("Current DrawObjectEventHandler value: " + (saveOptions.DrawObjectEventHandler == null ? "null" : "assigned"));
            
            // Establecer un nuevo controlador de eventos personalizado
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();
            
            // Esto activará el método Draw durante el renderizado
            workbook.Save("PropertyDrawObjectEventHandlerDemo.pdf", saveOptions);
            
            // Cambiar el controlador de eventos a null para demostrar la diferencia
            saveOptions.DrawObjectEventHandler = null;
            workbook.Save("PropertyDrawObjectEventHandlerDemo_NoHandler.pdf", saveOptions);
        }
    }
}
```

### Ver también

* class [DrawObjectEventHandler](../../../aspose.cells.rendering/drawobjecteventhandler/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



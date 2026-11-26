---
title: "DrawObject.TotalPages"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DrawObject. Indica el total de páginas en el renderizado actual"
type: docs
url: /es/net/aspose.cells.rendering/drawobject/totalpages/
---
## DrawObject.TotalPages property

Indica el total de páginas en el renderizado actual.

```csharp
public int TotalPages { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyTotalPagesDemo
    {
        // Manejador personalizado para capturar eventos DrawObject y leer la propiedad TotalPages
        private class TotalPagesHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                // Muestra el valor de la propiedad TotalPages
                Console.WriteLine($"Total Pages in Rendering: {drawObject.TotalPages}");
                Console.WriteLine($"Current Page: {drawObject.CurrentPage + 1}");
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine($"Sheet Index: {drawObject.SheetIndex}");
                Console.WriteLine();
            }
        }

        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Agrega datos de ejemplo para que el renderizado tenga sentido
                sheet.Cells["A1"].PutValue("Sample Data");
                sheet.Cells["A2"].PutValue("More Data");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Añade una forma para asegurar que se generen múltiples objetos de dibujo
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Configura las opciones de renderizado con nuestro controlador personalizado
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = false, // Allow multiple pages to demonstrate TotalPages
                    DrawObjectEventHandler = new TotalPagesHandler()
                };

                // Renderiza la hoja de cálculo - esto desencadenará los eventos DrawObject
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "TotalPagesDemo.png");

                // Guarda el libro de trabajo
                workbook.Save("TotalPagesDemo.xlsx");
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

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



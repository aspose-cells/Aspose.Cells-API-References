---
title: "DrawObject.Shape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DrawObject. Indica el objeto Shape al renderizar. Se pueden acceder a todas las propiedades de la forma"
type: docs
url: /es/net/aspose.cells.rendering/drawobject/shape/
---
## DrawObject.Shape property

Indica el objeto Shape al renderizar. Se pueden acceder a todas las propiedades de la forma.

```csharp
public Shape Shape { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyShapeDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Agrega datos de ejemplo para que el renderizado tenga sentido
                worksheet.Cells["A1"].Value = "Sample Data";
                worksheet.Cells["A2"].Value = "More Data";

                // Agregar una forma a la hoja de cálculo
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Configura las opciones de renderizado con un controlador personalizado
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new ShapePropertyHandler()
                };

                // Renderiza la hoja de cálculo - esto desencadenará los eventos DrawObject
                SheetRender sheetRender = new SheetRender(worksheet, renderOptions);
                sheetRender.ToImage(0, "ShapeDemo.png");

                // Guarda el libro de trabajo
                workbook.Save("ShapeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Controlador personalizado para capturar los eventos DrawObject y leer la propiedad Shape
        private class ShapePropertyHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                if (drawObject.Shape != null)
                {
                    Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                    Console.WriteLine($"Shape Name: {drawObject.Shape.Name}");
                    Console.WriteLine($"Shape Text: {drawObject.Shape.Text}");
                    Console.WriteLine($"Shape Width: {drawObject.Shape.Width} pixels");
                    Console.WriteLine($"Shape Height: {drawObject.Shape.Height} pixels");
                    Console.WriteLine($"Shape Type: {drawObject.Shape.AutoShapeType}");
                    Console.WriteLine();
                }
            }
        }
    }
}
```

### Ver también

* class [Shape](../../../aspose.cells.drawing/shape/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



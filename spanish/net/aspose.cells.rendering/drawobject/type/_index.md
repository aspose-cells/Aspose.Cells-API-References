---
title: "DrawObject.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DrawObject. Indica el tipo de DrawObject"
type: docs
url: /es/net/aspose.cells.rendering/drawobject/type/
---
## DrawObject.Type property

Indica el tipo de DrawObject.

```csharp
public DrawObjectEnum Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;

    public class DrawObjectPropertyTypeDemo
    {
        // Manejador personalizado que lee y muestra la propiedad Type de cada DrawObject
        private class TypeReaderHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");
                Console.WriteLine($"SheetIndex: {drawObject.SheetIndex}, Page: {drawObject.CurrentPage}/{drawObject.TotalPages}");
                Console.WriteLine();
            }
        }

        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo y acceder a la primera hoja de cálculo
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Rellena algunas celdas
                sheet.Cells["A1"].PutValue("Hello");
                sheet.Cells["A2"].PutValue("World");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Añade una forma para también generar objetos de dibujo de tipo shape‑type
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Establece opciones de renderizado con nuestro manejador de dibujo personalizado
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new TypeReaderHandler()
                };

                // Renderiza la hoja – esto activa los eventos DrawObject
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "DrawObjectTypeDemo.png");

                // Guardar el libro de trabajo (opcional)
                workbook.Save("DrawObjectTypeDemo.xlsx");
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

* enum [DrawObjectEnum](../../drawobjectenum/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



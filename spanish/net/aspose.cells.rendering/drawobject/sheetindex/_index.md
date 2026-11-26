---
title: "DrawObject.SheetIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DrawObject. Indica el índice de hoja actual de DrawObject"
type: docs
url: /es/net/aspose.cells.rendering/drawobject/sheetindex/
---
## DrawObject.SheetIndex property

Indica el índice de hoja actual de DrawObject.

```csharp
public int SheetIndex { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;

    // Controlador personalizado que lee y muestra el SheetIndex de cada DrawObject
    class SheetIndexReaderHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            Console.WriteLine($"DrawObject Type: {drawObject.Type}");
            Console.WriteLine($"SheetIndex: {drawObject.SheetIndex}");
            Console.WriteLine($"Page: {drawObject.CurrentPage + 1}/{drawObject.TotalPages}");
            Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");
            Console.WriteLine();
        }
    }

    public class DrawObjectPropertySheetIndexDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Rellena algunas celdas para que tengan contenido que renderizar
                sheet.Cells["A1"].PutValue("First");
                sheet.Cells["A2"].PutValue("Second");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Agrega una forma para que también se generen objetos de dibujo de forma
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Configura las opciones de renderizado con nuestro controlador personalizado
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new SheetIndexReaderHandler()
                };

                // Renderiza la hoja de cálculo – esto desencadena los eventos DrawObject
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "SheetIndexDemo.png");

                // Guardar el libro de trabajo (opcional)
                workbook.Save("SheetIndexDemo.xlsx");
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



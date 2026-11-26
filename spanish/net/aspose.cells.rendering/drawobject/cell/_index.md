---
title: "DrawObject.Cell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DrawObject. Indica el objeto Cell al renderizar. Se pueden acceder a todas las propiedades de la celda"
type: docs
url: /es/net/aspose.cells.rendering/drawobject/cell/
---
## DrawObject.Cell property

Indica el objeto Cell al renderizar. Se pueden acceder a todas las propiedades de la celda.

```csharp
public Cell Cell { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    // Controlador personalizado para capturar los eventos DrawObject y leer la propiedad Cell
    public class CellInfoDrawHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Salida de información básica del objeto de dibujo
            Console.WriteLine($"DrawObject Type: {drawObject.Type}");
            Console.WriteLine($"Location: ({x}, {y}), Size: ({width} x {height})");

            // Demostrar la lectura de la propiedad Cell de solo lectura
            if (drawObject.Cell != null)
            {
                var cell = drawObject.Cell;
                Console.WriteLine($"Cell Name: {cell.Name}");
                Console.WriteLine($"Cell Value: {cell.Value}");
                Console.WriteLine($"Cell Row: {cell.Row}, Column: {cell.Column}");
            }
        }
    }

    public class DrawObjectPropertyCellDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Agregar algunos datos de ejemplo a las celdas
                sheet.Cells["A1"].PutValue("Hello");
                sheet.Cells["A2"].PutValue("World");
                sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Agrega una forma para asegurar que también se generen los eventos de dibujo de forma
                Shape shape = sheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Configura las opciones de renderizado con nuestro controlador de dibujo personalizado
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new CellInfoDrawHandler()
                };

                // Renderiza la hoja de cálculo – esto desencadenará los eventos DrawObject
                SheetRender sheetRender = new SheetRender(sheet, renderOptions);
                sheetRender.ToImage(0, "DrawObjectCellDemo.png");

                // Guardar el libro de trabajo (opcional)
                workbook.Save("DrawObjectCellDemo.xlsx");
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

* class [Cell](../../../aspose.cells/cell/)
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)



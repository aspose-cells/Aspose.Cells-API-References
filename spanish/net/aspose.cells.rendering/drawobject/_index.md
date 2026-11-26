---
title: "Clase DrawObject"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Rendering.DrawObject. DrawObject se inicializará y devolverá al renderizar"
type: docs
url: /es/net/aspose.cells.rendering/drawobject/
---
## DrawObject class

DrawObject será inicializado y devuelto durante el renderizado.

```csharp
public class DrawObject
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Cell](../../aspose.cells.rendering/drawobject/cell/) { get; } | Indica el objeto Cell al renderizar. Se pueden acceder a todas las propiedades de la celda. |
| [CurrentPage](../../aspose.cells.rendering/drawobject/currentpage/) { get; } | Indica el índice de página de DrawObject. El índice de página se basa en cero. Una hoja contiene varias páginas al renderizar. |
| [ImageBytes](../../aspose.cells.rendering/drawobject/imagebytes/) { get; } | Indica los bytes de imagen del Chart o Shape renderizado al renderizar. |
| [Shape](../../aspose.cells.rendering/drawobject/shape/) { get; } | Indica el objeto Shape al renderizar. Se pueden acceder a todas las propiedades de la forma. |
| [SheetIndex](../../aspose.cells.rendering/drawobject/sheetindex/) { get; } | Indica el índice de hoja actual de DrawObject. |
| [TotalPages](../../aspose.cells.rendering/drawobject/totalpages/) { get; } | Indica el total de páginas en el renderizado actual. |
| [Type](../../aspose.cells.rendering/drawobject/type/) { get; } | Indica el tipo de DrawObject. |

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;

namespace AsposeCellsExamples
{
    // Implementación personalizada de DrawObjectEventHandler
    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            Console.WriteLine($"Drawing object at X: {x}, Y: {y}, Width: {width}, Height: {height}");
            Console.WriteLine($"Object Type: {drawObject.Type}");
            Console.WriteLine($"Sheet Index: {drawObject.SheetIndex}, Current Page: {drawObject.CurrentPage}, Total Pages: {drawObject.TotalPages}");

            if (drawObject.Cell != null)
            {
                Console.WriteLine($"Rendering Cell: {drawObject.Cell.Name}, Value: {drawObject.Cell.Value}");
            }

            if (drawObject.Shape != null)
            {
                Console.WriteLine($"Rendering Shape: {drawObject.Shape.Name}");
            }
        }
    }

    public class DrawObjectDemo
    {
        public static void RunDemo()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

            // Agregar una forma
            Aspose.Cells.Drawing.Shape shape = sheet.Shapes.AddShape(Aspose.Cells.Drawing.MsoDrawingType.Rectangle, 5, 0, 5, 0, 100, 100);
            shape.Text = "Sample Shape";

            // Crear una instancia de CustomDrawObjectEventHandler
            CustomDrawObjectEventHandler drawObjectEventHandler = new CustomDrawObjectEventHandler();

            // Establecer opciones de imagen o impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                DrawObjectEventHandler = drawObjectEventHandler,
                OnePagePerSheet = true,
                ImageType = Aspose.Cells.Drawing.ImageType.Png
            };

            // Renderizar la hoja a una imagen
            SheetRender sr = new SheetRender(sheet, options);
            sr.ToImage(0, "DrawObjectDemo.png");

            // Guarda el libro de trabajo
            workbook.Save("DrawObjectDemo.xlsx");
            workbook.Save("DrawObjectDemo.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)



---
title: "Enumeración DrawObjectEnum"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Rendering.DrawObjectEnum. Indica Celda o Imagen de DrawObject"
type: docs
url: /es/net/aspose.cells.rendering/drawobjectenum/
---
## DrawObjectEnum enumeration

Indica la celda o la imagen del DrawObject.

```csharp
public enum DrawObjectEnum
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Image | `0` | Indica que DrawObject es una Imagen |
| Cell | `1` | indica que DrawObject es una Celda |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassDrawObjectEnumDemo
    {
        public static void Run()
        {
            // Crea un libro y añade datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Cell");

            // Crea un objeto PdfSaveOptions
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Crea un DrawObjectEventHandler personalizado
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();

            // Guarda el libro en PDF con el manejador personalizado
            workbook.Save("output.pdf", saveOptions);
        }
    }

    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Comprueba si el objeto de dibujo es una celda
            if (drawObject.Type == DrawObjectEnum.Cell)
            {
                Cell cell = drawObject.Cell;
                
                // Muestra información de la celda
                Console.WriteLine($"Drawing Cell - Row: {cell.Row}, Column: {cell.Column}");
                Console.WriteLine($"Position: ({x}, {y}), Size: {width}x{height}");
                
                // Manejo especial para la celda A1
                if (cell.Row == 0 && cell.Column == 0)
                {
                    Console.WriteLine("This is cell A1");
                }
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)



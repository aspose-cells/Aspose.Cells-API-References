---
title: "HtmlSaveOptions.IgnoreInvisibleShapes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exportan esas formas no visibles"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/ignoreinvisibleshapes/
---
## HtmlSaveOptions.IgnoreInvisibleShapes property

Indica si se exportan las formas que no son visibles

```csharp
public bool IgnoreInvisibleShapes { get; set; }
```

### Observaciones

El valor predeterminado es false.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIgnoreInvisibleShapesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con una hoja de cálculo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar formas visibles e invisibles
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 50, 50);
            shape1.IsHidden = false;
            Shape shape2 = worksheet.Shapes.AddRectangle(1, 0, 100, 100, 50, 50);
            shape2.IsHidden = true;

            // Guardar con IgnoreInvisibleShapes = true (predeterminado)
            HtmlSaveOptions saveOptions1 = new HtmlSaveOptions();
            saveOptions1.IgnoreInvisibleShapes = true;
            workbook.Save("output_ignore_invisible.html", saveOptions1);

            // Guardar con IgnoreInvisibleShapes = false
            HtmlSaveOptions saveOptions2 = new HtmlSaveOptions();
            saveOptions2.IgnoreInvisibleShapes = false;
            workbook.Save("output_include_invisible.html", saveOptions2);

            Console.WriteLine("HTML files saved with different IgnoreInvisibleShapes settings.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



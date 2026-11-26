---
title: "MsoFillFormat.IsVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFillFormat. Indica si hay relleno"
type: docs
url: /es/net/aspose.cells.drawing/msofillformat/isvisible/
---
## MsoFillFormat.IsVisible property

Indica si hay relleno.

```csharp
public bool IsVisible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma de ejemplo
            Shape shape1 = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 100, 150);

            // Establecer la visibilidad del relleno para shape1 (visible)
            shape1.FillFormat.IsVisible = true;
            shape1.FillFormat.ForeColor = System.Drawing.Color.Red;
            
            // Establecer la visibilidad del relleno para shape2 (invisible)
            shape2.FillFormat.IsVisible = false;

            // Demostrar el uso de la propiedad IsVisible
            Console.WriteLine("Shape1 Fill Visible: " + shape1.FillFormat.IsVisible);
            Console.WriteLine("Shape2 Fill Visible: " + shape2.FillFormat.IsVisible);

            // Comparar la visibilidad del relleno entre formas
            if (shape1.FillFormat.IsVisible && shape2.FillFormat.IsVisible)
            {
                Console.WriteLine("Both shapes have visible fills");
            }
            else
            {
                Console.WriteLine("At least one shape has invisible fill");
            }

            // Guarda el libro de trabajo
            workbook.Save("MsoFillFormatIsVisibleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



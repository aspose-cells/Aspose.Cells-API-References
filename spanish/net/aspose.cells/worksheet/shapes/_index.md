---
title: "Worksheet.Shapes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Devuelve todas las formas de dibujo en esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/shapes/
---
## Worksheet.Shapes property

Devuelve todas las formas de dibujo en esta hoja de cálculo.

```csharp
public ShapeCollection Shapes { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyShapesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar algunas formas a la hoja de cálculo
            sheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            sheet.Shapes.AddLine(2, 0, 100, 100, 100, 1);
            
            // Modificar propiedades de la forma
            for (int i = 0; i < sheet.Shapes.Count; i++)
            {
                Aspose.Cells.Drawing.Shape shape = sheet.Shapes[i];
                Console.WriteLine($"Shape {i}: Type={shape.Type}, Name={shape.Name}");
                
                // Actualizar propiedades de la primera forma
                if (i == 0)
                {
                    shape.Name = "MyRectangle";
                    shape.FillFormat.ForeColor = System.Drawing.Color.Red;
                }
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ShapesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



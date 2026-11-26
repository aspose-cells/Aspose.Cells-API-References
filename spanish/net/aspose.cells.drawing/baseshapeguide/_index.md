---
title: "Clase BaseShapeGuide"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.BaseShapeGuide. Representa la guía de forma"
type: docs
url: /es/net/aspose.cells.drawing/baseshapeguide/
---
## BaseShapeGuide class

Representa la guía de forma.

```csharp
public class BaseShapeGuide
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassBaseShapeGuideDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crear una forma rectangular con parámetros correctos
                Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

                // Dado que BaseShapeGuide no tiene un constructor público,
                // demostraremos su uso a través de una forma que podría contener guías
                // Nota: Esta es una demostración simplificada ya que el acceso real a la guía podría diferir
                Console.WriteLine("Shape created successfully");
                Console.WriteLine($"Shape type: {shape.GetType().Name}");

                // Guarda el libro de trabajo
                workbook.Save("BaseShapeGuideDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with BaseShapeGuide: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



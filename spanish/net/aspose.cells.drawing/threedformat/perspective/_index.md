---
title: "ThreeDFormat.Perspective"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Obtiene y establece el ángulo desde el cual se puede ver un objeto ThreeDFormat"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/perspective/
---
## ThreeDFormat.Perspective property

Obtiene y establece el ángulo desde el cual se puede ver un objeto ThreeDFormat.

```csharp
public double Perspective { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyPerspectiveDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar el formato 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 0, 0, 200, 100);
            
            // Obtener el formato 3D de la forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mostrar el valor de perspectiva actual
            Console.WriteLine("Current Perspective value: " + threeDFormat.Perspective);

            // Establecer nuevo valor de perspectiva (0 a 120 grados)
            threeDFormat.Perspective = 45;
            Console.WriteLine("Perspective set to: " + threeDFormat.Perspective);

            // Aplicar otros efectos 3D para visualizar mejor el cambio de perspectiva
            threeDFormat.ExtrusionHeight = 15;
            threeDFormat.ContourWidth = 2;
            threeDFormat.RotationX = 20;
            threeDFormat.RotationY = 30;

            // Guardar el libro de trabajo para ver los efectos
            workbook.Save("ThreeDFormatPerspectiveDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



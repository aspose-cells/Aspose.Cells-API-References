---
title: "ThreeDFormat.Z"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Define la distancia desde el suelo para la forma 3D"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/z/
---
## ThreeDFormat.Z property

Define la distancia desde el suelo para la forma 3D.

```csharp
public double Z { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyZDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar el formato 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 0, 0, 200, 100);
            
            // Acceder al ThreeDFormat de la forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mostrar el valor actual de Z (distancia desde el suelo)
            Console.WriteLine("Current Z value: " + threeDFormat.Z);

            // Establecer nuevo valor de Z para mover la forma más lejos del suelo
            threeDFormat.Z = 20;
            Console.WriteLine("New Z value: " + threeDFormat.Z);

            // Configurar otras propiedades 3D para que el efecto sea visible
            threeDFormat.ExtrusionHeight = 30;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;

            // Guardar el libro de trabajo para ver el efecto 3D
            workbook.Save("ThreeDFormatPropertyZDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



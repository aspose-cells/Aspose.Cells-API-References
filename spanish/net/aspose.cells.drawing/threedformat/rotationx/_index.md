---
title: "ThreeDFormat.RotationX"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Obtiene y establece la rotación de la forma extruida alrededor del eje x en grados"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/rotationx/
---
## ThreeDFormat.RotationX property

Obtiene y establece la rotación de la forma extruida alrededor del eje x en grados.

```csharp
public double RotationX { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationXDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar el formato 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 2, 2, 200, 100, 100);
            
            // Obtener formato 3D (no es necesario "activar" los efectos 3D - solo establezca las propiedades)
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mostrar el valor actual de RotationX
            Console.WriteLine("Current RotationX value: " + threeDFormat.RotationX);

            // Establecer nuevo valor de RotationX (rotación alrededor del eje x en grados)
            threeDFormat.RotationX = 45;
            Console.WriteLine("New RotationX value: " + threeDFormat.RotationX);

            // Establecer otras propiedades 3D para que la rotación sea visible
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;

            // Guardar el libro de trabajo para ver los efectos
            workbook.Save("ThreeDFormatRotationXDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



---
title: "ThreeDFormat.RotationY"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Obtiene y establece la rotación de la forma extruida alrededor del eje Y en grados"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/rotationy/
---
## ThreeDFormat.RotationY property

Obtiene y establece la rotación de la forma extruida alrededor del eje y en grados.

```csharp
public double RotationY { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationYDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar el formato 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 100, 150, 150);
            shape.Text = "3D Rotation Demo";
            
            // Acceder al ThreeDFormat de la forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mostrar el valor actual de RotationY
            Console.WriteLine("Current RotationY value: " + threeDFormat.RotationY);

            // Establecer nuevos valores de RotationY y demostrar los efectos
            threeDFormat.RotationY = 15;
            Console.WriteLine("Shape rotated 15 degrees around Y-axis");

            // Aplicar otras propiedades 3D para que el efecto sea visible
            threeDFormat.ExtrusionHeight = 5;
            threeDFormat.ContourWidth = 1;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;

            // Guardar el libro de trabajo para mostrar los efectos
            workbook.Save("ThreeDFormatRotationYDemo.xlsx");

            // Cambiar la rotación nuevamente y guardar otra versión
            threeDFormat.RotationY = 45;
            workbook.Save("ThreeDFormatRotationYDemo_45degrees.xlsx");
        }
    }
}
```

### Ver también

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



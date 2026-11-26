---
title: "ThreeDFormat.RotationZ"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Obtiene y establece la rotación de la forma extruida alrededor del eje z en grados"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/rotationz/
---
## ThreeDFormat.RotationZ property

Obtiene y establece la rotación de la forma extruida alrededor del eje z en grados.

```csharp
public double RotationZ { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationZDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar el formato 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 0, 100, 150);
            shape.Text = "3D Rotation Demo";
            
            // Acceder al ThreeDFormat de la forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mostrar el valor actual de RotationZ
            Console.WriteLine("Current RotationZ value: " + threeDFormat.RotationZ);

            // Establecer nuevos valores de RotationZ y demostrar los efectos
            threeDFormat.RotationZ = 45;
            Console.WriteLine("Shape rotated 45 degrees around Z-axis");

            // Aplicar otras propiedades 3D para que la rotación sea visible
            threeDFormat.ExtrusionHeight = 15;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;

            // Guardar el libro de trabajo con los efectos 3D
            workbook.Save("ThreeDFormatRotationZDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



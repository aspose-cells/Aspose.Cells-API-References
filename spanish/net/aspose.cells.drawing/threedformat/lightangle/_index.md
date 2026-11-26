---
title: "ThreeDFormat.LightAngle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Obtiene y establece el ángulo de las luces de extrusión"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/lightangle/
---
## ThreeDFormat.LightAngle property

Obtiene y establece el ángulo de las luces de extrusión.

```csharp
public double LightAngle { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightAngleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar el formato 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 200, 100, 0, 0);
            shape.Text = "3D Format Demo";
            
            // Acceder al ThreeDFormat de la forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mostrar el valor actual de LightAngle
            Console.WriteLine("Current LightAngle value: " + threeDFormat.LightAngle);

            // Establecer nuevo valor de LightAngle (0 a 359,9 grados)
            threeDFormat.LightAngle = 45;
            Console.WriteLine("New LightAngle value: " + threeDFormat.LightAngle);

            // Configurar otras propiedades 3D para ver el efecto de LightAngle
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.Material = PresetMaterialType.Plastic;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.LightingDirection = LightRigDirectionType.Top;

            // Guardar el libro de trabajo para ver los efectos
            workbook.Save("ThreeDFormatLightAngleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



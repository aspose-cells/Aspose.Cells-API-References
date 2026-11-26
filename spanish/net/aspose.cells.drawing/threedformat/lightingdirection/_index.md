---
title: "ThreeDFormat.LightingDirection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Obtiene y establece la dirección desde la cual se orienta la configuración de luz en relación con la escena"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/lightingdirection/
---
## ThreeDFormat.LightingDirection property

Obtiene y establece la dirección desde la cual se orienta la configuración de luz en relación con la escena.

```csharp
public LightRigDirectionType LightingDirection { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightingDirectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar el formato 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 100);
            shape.Text = "3D Lighting Direction Demo";
            
            // Obtener el ThreeDFormat de la forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Establecer propiedades 3D iniciales
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.Material = PresetMaterialType.Plastic;

            // Mostrar la dirección de iluminación actual
            Console.WriteLine("Current LightingDirection: " + threeDFormat.LightingDirection);

            // Cambiar la dirección de iluminación y observar los efectos
            threeDFormat.LightingDirection = LightRigDirectionType.TopLeft;
            Console.WriteLine("Changed LightingDirection to TopLeft");

            // Cambiar a otra dirección
            threeDFormat.LightingDirection = LightRigDirectionType.BottomRight;
            Console.WriteLine("Changed LightingDirection to BottomRight");

            // Guardar el libro de trabajo para ver los efectos visuales
            workbook.Save("ThreeDFormatLightingDirectionDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [LightRigDirectionType](../../lightrigdirectiontype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



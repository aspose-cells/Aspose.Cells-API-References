---
title: "ThreeDFormat.Lighting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Obtiene y establece el tipo de configuración de luz"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/lighting/
---
## ThreeDFormat.Lighting property

Obtiene y establece el tipo de configuración de luz.

```csharp
public LightRigType Lighting { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyLightingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar el formato 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 200);
            shape.Text = "3D Lighting Demo";
            
            // Obtener el ThreeDFormat de la forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mostrar el valor de iluminación actual
            Console.WriteLine("Current Lighting value: " + threeDFormat.Lighting);

            // Establecer diferentes tipos de iluminación y observar los efectos
            threeDFormat.Lighting = LightRigType.BrightRoom;
            Console.WriteLine("Changed to BrightRoom lighting");

            // Aplicar algunas otras propiedades 3D para ver mejor el efecto de iluminación
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;

            // Guardar con el primer tipo de iluminación
            workbook.Save("BrightRoomLighting.xlsx");

            // Cambiar a otro tipo de iluminación
            threeDFormat.Lighting = LightRigType.Sunset;
            Console.WriteLine("Changed to Sunset lighting");
            workbook.Save("SunsetLighting.xlsx");

            // Cambiar a un tercer tipo de iluminación
            threeDFormat.Lighting = LightRigType.ThreePoint;
            Console.WriteLine("Changed to ThreePoint lighting");
            workbook.Save("ThreePointLighting.xlsx");
        }
    }
}
```

### Ver también

* enum [LightRigType](../../lightrigtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



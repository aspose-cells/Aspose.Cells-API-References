---
title: "ThreeDFormat.PresetCameraType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Obtiene y establece el tipo de cámara predefinida de la extrusión"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/presetcameratype/
---
## ThreeDFormat.PresetCameraType property

Obtiene y establece el tipo de cámara preestablecida de extrusión.

```csharp
public PresetCameraType PresetCameraType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyPresetCameraTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar el formato 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 0, 0, 200, 200);
            
            // Obtener el ThreeDFormat de la forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mostrar el valor actual de PresetCameraType
            Console.WriteLine("Current PresetCameraType: " + threeDFormat.PresetCameraType);

            // Establecer un nuevo valor de PresetCameraType
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveHeroicLeftFacing;

            // Aplicar un formato 3D adicional para que el efecto sea visible
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Material = PresetMaterialType.Plastic;
            threeDFormat.Lighting = LightRigType.ThreePoint;
            threeDFormat.LightingDirection = LightRigDirectionType.Top;

            // Mostrar el nuevo valor de PresetCameraType
            Console.WriteLine("New PresetCameraType: " + threeDFormat.PresetCameraType);

            // Guardar el libro de trabajo para mostrar el efecto
            workbook.Save("ThreeDFormatPresetCameraTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PresetCameraType](../../presetcameratype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



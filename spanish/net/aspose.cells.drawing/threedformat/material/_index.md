---
title: "ThreeDFormat.Material"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Representa el material preestablecido que se combina con las propiedades de iluminación para dar el aspecto final y la sensación de una forma"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/material/
---
## ThreeDFormat.Material property

Representa el material preestablecido que se combina con las propiedades de iluminación para dar el aspecto y la sensación final de una forma.

```csharp
public PresetMaterialType Material { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyMaterialDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar el formato 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);
            shape.Text = "3D Material Demo";
            
            // Acceder al ThreeDFormat de la forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Mostrar el valor actual del material
            Console.WriteLine("Current Material value: " + threeDFormat.Material);

            // Establezca diferentes tipos de material y observe los efectos
            threeDFormat.Material = PresetMaterialType.Metal;
            Console.WriteLine("Material changed to Metal");

            threeDFormat.Material = PresetMaterialType.Plastic;
            Console.WriteLine("Material changed to Plastic");

            threeDFormat.Material = PresetMaterialType.Matte;
            Console.WriteLine("Material changed to Matte");

            // Configure otras propiedades 3D para ver mejor el efecto del material
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;
            threeDFormat.RotationX = 20;
            threeDFormat.RotationY = 30;

            // Guardar el libro de trabajo con los efectos 3D
            workbook.Save("ThreeDFormatMaterialDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PresetMaterialType](../../presetmaterialtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



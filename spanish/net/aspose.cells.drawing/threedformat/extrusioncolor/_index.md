---
title: "ThreeDFormat.ExtrusionColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Obtiene el color de extrusión en una forma"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/extrusioncolor/
---
## ThreeDFormat.ExtrusionColor property

Obtiene el color de extrusión en una forma.

```csharp
public CellsColor ExtrusionColor { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyExtrusionColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar el formato 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 100);
            shape.Text = "3D ExtrusionColor Demo";
            
            // Obtener el ThreeDFormat de la forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Configurar propiedades 3D básicas para que la extrusión sea visible
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Material = PresetMaterialType.Plastic;

            try
            {
                // Obtener y mostrar el valor de ExtrusionColor
                CellsColor extrusionColor = threeDFormat.ExtrusionColor;
                Console.WriteLine("ExtrusionColor properties:");
                Console.WriteLine($"Type: {extrusionColor.Type}");
                Console.WriteLine($"Color (RGB): {extrusionColor.Color}");
                Console.WriteLine($"Transparency: {extrusionColor.Transparency}");

                // Guardar el libro de trabajo para ver los efectos 3D
                workbook.Save("ThreeDFormatExtrusionColorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



---
title: "ThreeDFormat.ContourColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Obtiene y establece el color de contorno en una forma"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/contourcolor/
---
## ThreeDFormat.ContourColor property

Obtiene y establece el color del contorno en una forma.

```csharp
public CellsColor ContourColor { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyContourColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar el formato 3D
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 200, 100, 0, 0);
            shape.Text = "3D ContourColor Demo";
            
            // Obtener el ThreeDFormat de la forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Configurar propiedades 3D básicas
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ContourWidth = 2;

            try
            {
                // Obtener el valor actual de ContourColor
                CellsColor contourColor = threeDFormat.ContourColor;
                Console.WriteLine($"Initial ContourColor - Type: {contourColor.Type}, ARGB: {contourColor.Argb}");

                // Crear un nuevo color modificando uno existente
                contourColor.Argb = System.Drawing.Color.Red.ToArgb();
                contourColor.Transparency = 0.5;
                threeDFormat.ContourColor = contourColor;

                // Mostrar el nuevo valor de ContourColor
                Console.WriteLine($"New ContourColor - Type: {threeDFormat.ContourColor.Type}, ARGB: {threeDFormat.ContourColor.Argb}");

                // Guardar el libro de trabajo para ver los efectos
                workbook.Save("ThreeDFormatContourColorDemo.xlsx");
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



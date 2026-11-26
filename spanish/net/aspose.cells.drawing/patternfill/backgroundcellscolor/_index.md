---
title: "PatternFill.BackgroundCellsColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PatternFill. Obtiene y establece el objeto CellsColor de primer plano"
type: docs
url: /es/net/aspose.cells.drawing/patternfill/backgroundcellscolor/
---
## PatternFill.BackgroundCellsColor property

Obtiene y establece el objeto [`CellsColor`](../../../aspose.cells/cellscolor/) de primer plano.

```csharp
public CellsColor BackgroundCellsColor { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyBackgroundCellsColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Añade una forma rectangular para demostrar el relleno de patrón
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            try
            {
                // Establece el tipo de relleno a patrón
                shape.Fill.FillType = FillType.Pattern;

                // Obtén la instancia de PatternFill
                PatternFill patternFill = shape.Fill.PatternFill;

                // Establece el tipo de patrón y los colores
                patternFill.Pattern = FillPattern.WideDownwardDiagonal;
                patternFill.ForegroundColor = Color.Red;
                patternFill.BackgroundColor = Color.Yellow;

                // Accede y modifica las propiedades de BackgroundCellsColor
                patternFill.BackgroundCellsColor.Color = Color.Blue;
                patternFill.BackgroundCellsColor.Argb = Color.Blue.ToArgb();
                patternFill.BackgroundCellsColor.Transparency = 0.3;

                // Muestra las propiedades de BackgroundCellsColor
                Console.WriteLine("BackgroundCellsColor Type: " + patternFill.BackgroundCellsColor.Type);
                Console.WriteLine("BackgroundCellsColor Color: " + patternFill.BackgroundCellsColor.Color);
                Console.WriteLine("BackgroundCellsColor ARGB: " + patternFill.BackgroundCellsColor.Argb);
                Console.WriteLine("BackgroundCellsColor Transparency: " + patternFill.BackgroundCellsColor.Transparency);

                // Guarda el libro de trabajo
                workbook.Save("BackgroundCellsColorDemo.xlsx");
                Console.WriteLine("BackgroundCellsColor demonstration completed successfully.");
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
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



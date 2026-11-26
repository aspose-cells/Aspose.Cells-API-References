---
title: "PatternFill.ForegroundCellsColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PatternFill. Obtiene y establece el objeto CellsColor de primer plano"
type: docs
url: /es/net/aspose.cells.drawing/patternfill/foregroundcellscolor/
---
## PatternFill.ForegroundCellsColor property

Obtiene y establece el objeto [`CellsColor`](../../../aspose.cells/cellscolor/) de primer plano.

```csharp
public CellsColor ForegroundCellsColor { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForegroundCellsColorDemo
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

                // Crea un objeto CellsColor para el primer plano usando la propiedad Color
                // Dado que CellsColor no tiene un constructor público, utilizaremos el ForegroundCellsColor existente
                // y modifica sus propiedades directamente
                patternFill.ForegroundCellsColor.Color = Color.Blue;
                patternFill.ForegroundCellsColor.Argb = Color.Blue.ToArgb();

                // Muestra las propiedades de ForegroundCellsColor
                Console.WriteLine("ForegroundCellsColor Type: " + patternFill.ForegroundCellsColor.Type);
                Console.WriteLine("ForegroundCellsColor Color: " + patternFill.ForegroundCellsColor.Color);
                Console.WriteLine("ForegroundCellsColor ARGB: " + patternFill.ForegroundCellsColor.Argb);

                // Guarda el libro de trabajo
                workbook.Save("ForegroundCellsColorDemo.xlsx");
                Console.WriteLine("ForegroundCellsColor demonstration completed successfully.");
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



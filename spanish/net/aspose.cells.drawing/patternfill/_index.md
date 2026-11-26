---
title: "Clase PatternFill"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.PatternFill class. Encapsula el objeto que representa el formato de relleno de patrón"
type: docs
url: /es/net/aspose.cells.drawing/patternfill/
---
## PatternFill class

Encapsula el objeto que representa el formato de relleno de patrón

```csharp
public class PatternFill : Fill
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackgroundCellsColor](../../aspose.cells.drawing/patternfill/backgroundcellscolor/) { get; set; } | Obtiene y establece el objeto de primer plano [`CellsColor`](../../aspose.cells/cellscolor/). |
| [BackgroundColor](../../aspose.cells.drawing/patternfill/backgroundcolor/) { get; set; } | Obtiene o establece el Color de fondo del [`Area`](../area/). |
| [BackTransparency](../../aspose.cells.drawing/patternfill/backtransparency/) { get; set; } | Obtiene o establece la transparencia del color de fondo. |
| [ForegroundCellsColor](../../aspose.cells.drawing/patternfill/foregroundcellscolor/) { get; set; } | Obtiene y establece el objeto de primer plano [`CellsColor`](../../aspose.cells/cellscolor/). |
| [ForegroundColor](../../aspose.cells.drawing/patternfill/foregroundcolor/) { get; set; } | Obtiene o establece el Color de primer plano. |
| [ForeTransparency](../../aspose.cells.drawing/patternfill/foretransparency/) { get; set; } | Obtiene o establece la transparencia del color de primer plano. |
| [Pattern](../../aspose.cells.drawing/patternfill/pattern/) { get; set; } | Obtiene o establece el tipo de patrón de relleno |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Hereda de [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Obtiene el código hash.(Hereda de [`Fill`](../fill/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassPatternFillDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un estilo para la celda usando el patrón BackgroundType
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.DiagonalStripe;
            style.ForegroundColor = Color.LightBlue;
            style.BackgroundColor = Color.DarkBlue;

            worksheet.Cells["B2"].SetStyle(style);
            worksheet.Cells["B2"].PutValue("PatternFill Demo");

            // Crear forma y configurar su relleno de patrón
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 100);
            shape.Fill.FillType = FillType.Pattern;
            
            PatternFill shapePatternFill = shape.Fill.PatternFill;
            shapePatternFill.Pattern = FillPattern.DiagonalBrick;
            shapePatternFill.ForegroundColor = Color.LightBlue;
            shapePatternFill.BackgroundColor = Color.DarkBlue;
            shapePatternFill.ForeTransparency = 0.2;
            shapePatternFill.BackTransparency = 0.3;

            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.Color = Color.Gold;
            shapePatternFill.ForegroundCellsColor = cellsColor;

            workbook.Save("PatternFillDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



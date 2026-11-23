---
title: "Classe PatternFill"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.PatternFill. Encapsule l'objet qui représente le format de remplissage de motif"
type: docs
url: /fr/net/aspose.cells.drawing/patternfill/
---
## PatternFill class

Encapsule l'objet qui représente le format de remplissage de motif

```csharp
public class PatternFill : Fill
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BackgroundCellsColor](../../aspose.cells.drawing/patternfill/backgroundcellscolor/) { get; set; } | Obtient et définit l'objet de premier plan [`CellsColor`](../../aspose.cells/cellscolor/). |
| [BackgroundColor](../../aspose.cells.drawing/patternfill/backgroundcolor/) { get; set; } | Obtient ou définit la couleur d'arrière-plan du [`Area`](../area/). |
| [BackTransparency](../../aspose.cells.drawing/patternfill/backtransparency/) { get; set; } | Obtient ou définit la transparence de la couleur d'arrière-plan. |
| [ForegroundCellsColor](../../aspose.cells.drawing/patternfill/foregroundcellscolor/) { get; set; } | Obtient et définit l'objet de premier plan [`CellsColor`](../../aspose.cells/cellscolor/). |
| [ForegroundColor](../../aspose.cells.drawing/patternfill/foregroundcolor/) { get; set; } | Obtient ou définit la couleur de premier plan. |
| [ForeTransparency](../../aspose.cells.drawing/patternfill/foretransparency/) { get; set; } | Obtient ou définit la transparence de la couleur de premier plan. |
| [Pattern](../../aspose.cells.drawing/patternfill/pattern/) { get; set; } | Obtient ou définit le type de motif de remplissage |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Hérité de [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Obtient le code de hachage.(Hérité de [`Fill`](../fill/).) |

### Exemples

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

            // Créez un style pour la cellule en utilisant le motif BackgroundType
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.DiagonalStripe;
            style.ForegroundColor = Color.LightBlue;
            style.BackgroundColor = Color.DarkBlue;

            worksheet.Cells["B2"].SetStyle(style);
            worksheet.Cells["B2"].PutValue("PatternFill Demo");

            // Créer une forme et configurer son remplissage à motif
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

### Voir aussi

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



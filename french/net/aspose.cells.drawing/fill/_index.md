---
title: "Classe Fill"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.Fill. Représente le format de remplissage de la forme"
type: docs
url: /fr/net/aspose.cells.drawing/fill/
---
## Fill class

Représente le format de remplissage de la forme.

```csharp
public abstract class Fill
```

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | / |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Obtient le code de hachage. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassFillDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 150);
            // Définir le type de remplissage sur solide et modifier la couleur
            rectangle.Fill.FillType = FillType.Solid;
            rectangle.Fill.SolidFill.Color = Color.LightBlue;

            Shape oval = worksheet.Shapes.AddOval(2, 0, 0, 0, 100, 150);
            // Utiliser la méthode de remplissage en dégradé directement sur FillFormat
            oval.Fill.SetTwoColorGradient(Color.DarkBlue, Color.SkyBlue, GradientStyleType.Vertical, 0);

            workbook.Save("DrawingClassFillDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



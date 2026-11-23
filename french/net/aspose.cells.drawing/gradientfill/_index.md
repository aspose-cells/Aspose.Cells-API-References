---
title: "Classe GradientFill"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.GradientFill. Représente le remplissage en dégradé"
type: docs
url: /fr/net/aspose.cells.drawing/gradientfill/
---
## GradientFill class

Représente le remplissage en dégradé.

```csharp
public class GradientFill : Fill
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Angle](../../aspose.cells.drawing/gradientfill/angle/) { get; set; } | L'angle du remplissage linéaire. |
| [DirectionType](../../aspose.cells.drawing/gradientfill/directiontype/) { get; } | Obtient le type de direction du dégradé. |
| [FillType](../../aspose.cells.drawing/gradientfill/filltype/) { get; } | Obtient le type de remplissage en dégradé. |
| [GradientStops](../../aspose.cells.drawing/gradientfill/gradientstops/) { get; } | Représente la collection de points d'arrêt du dégradé. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Hérité de [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Obtient le code de hachage.(Hérité de [`Fill`](../fill/).) |
| [SetGradient](../../aspose.cells.drawing/gradientfill/setgradient/)(GradientFillType, double, GradientDirectionType) | Définir le type et la direction du remplissage en dégradé. |
| [SetOneColorGradient](../../aspose.cells.drawing/gradientfill/setonecolorgradient/)(Color, double, GradientStyleType, int) | Définit le remplissage spécifié comme un dégradé à une couleur. S'applique uniquement à Excel 2007. |
| [SetPresetThemeGradient](../../aspose.cells.drawing/gradientfill/setpresetthemegradient/)(PresetThemeGradientType, ThemeColorType) | Définit le remplissage en dégradé de thème prédéfini. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Définit le remplissage spécifié comme un dégradé à deux couleurs. S'applique uniquement à Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Définit le remplissage spécifié comme un dégradé à deux couleurs. S'applique uniquement à Excel 2007. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassGradientFillDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire à la feuille de calcul avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 150, 100);

            // Définir le type de remplissage sur dégradé pour accéder aux propriétés du remplissage en dégradé
            shape.Fill.FillType = FillType.Gradient;

            // Obtenir l'instance de remplissage en dégradé existante à partir de la forme
            GradientFill gradientFill = shape.Fill.GradientFill;

            // Configurer le dégradé avec deux couleurs en utilisant l'instance existante
            gradientFill.SetTwoColorGradient(
                Color.LightSkyBlue,  // First color
                Color.DarkBlue,      // Second color
                GradientStyleType.Horizontal, // Gradient style
                1                    // Variant
            );

            // Enregistrez le classeur
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



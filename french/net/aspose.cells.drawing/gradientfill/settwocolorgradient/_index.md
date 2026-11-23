---
title: "GradientFill.SetTwoColorGradient"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GradientFill. Définit le remplissage spécifié à un dégradé bicolore. S'applique uniquement à Excel 2007"
type: docs
url: /fr/net/aspose.cells.drawing/gradientfill/settwocolorgradient/
---
## SetTwoColorGradient(Color, Color, GradientStyleType, int) {#settwocolorgradient_1}

Définit le remplissage spécifié comme un dégradé à deux couleurs. S'applique uniquement à Excel 2007.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType style, int variant)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| color1 | Color | Une couleur de dégradé. |
| color2 | Color | Deux couleurs de dégradé. |
| style | GradientStyleType | Style d’ombrage du dégradé. |
| variant | Int32 | La variante du dégradé. Peut être une valeur de 1 à 4, correspondant à l'une des quatre variantes de l'onglet Dégradé dans la boîte de dialogue Effets de remplissage. Si le style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientFillMethodSetTwoColorGradientWithColorColorGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour appliquer un remplissage en dégradé
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Définir le type de remplissage sur dégradé
                shape.Fill.FillType = FillType.Gradient;

                // Obtenir le remplissage en dégradé
                GradientFill gradientFill = shape.Fill.GradientFill;
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // Appeler SetTwoColorGradient avec des paramètres réalistes
                gradientFill.SetTwoColorGradient(
                    Color.Red,          // color1
                    Color.Blue,         // color2
                    GradientStyleType.DiagonalDown,  // style
                    1);                 // variant

                Console.WriteLine("SetTwoColorGradient method called successfully with parameters (Red, Blue, DiagonalDown, 1)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTwoColorGradient: {ex.Message}");
            }

            // Enregistrez le classeur pour démontrer l'effet
            workbook.Save("SetTwoColorGradientDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetTwoColorGradient(Color, double, Color, double, GradientStyleType, int) {#settwocolorgradient}

Définit le remplissage spécifié comme un dégradé à deux couleurs. S'applique uniquement à Excel 2007.

```csharp
public void SetTwoColorGradient(Color color1, double transparency1, Color color2, 
    double transparency2, GradientStyleType style, int variant)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| color1 | Color | Une couleur de dégradé. |
| transparency1 | Double | Le degré de transparence de la couleur1, exprimé par une valeur comprise entre 0,0 (opaque) et 1,0 (transparent). |
| color2 | Color | Deux couleurs de dégradé. |
| transparency2 | Double | Le degré de transparence de la couleur2, exprimé par une valeur comprise entre 0,0 (opaque) et 1,0 (transparent). |
| style | GradientStyleType | Style d’ombrage du dégradé. |
| variant | Int32 | La variante du dégradé. Peut être une valeur de 1 à 4, correspondant à l'une des quatre variantes de l'onglet Dégradé dans la boîte de dialogue Effets de remplissage. Si le style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientFillMethodSetTwoColorGradientWithColorDoubleColorDoubleGradient297116Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour appliquer un remplissage en dégradé
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Définir le type de remplissage sur dégradé
                shape.Fill.FillType = FillType.Gradient;

                // Obtenir le remplissage en dégradé
                GradientFill gradientFill = shape.Fill.GradientFill;
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // Appeler SetTwoColorGradient avec des paramètres réalistes
                gradientFill.SetTwoColorGradient(
                    Color.Red,          // color1
                    0.5,                // transparency1 (50% transparent)
                    Color.Blue,         // color2
                    0.3,                // transparency2 (30% transparent)
                    GradientStyleType.Horizontal,  // style
                    2);                 // variant

                Console.WriteLine("SetTwoColorGradient method called successfully with parameters (Red, 0.5, Blue, 0.3, Horizontal, 2)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTwoColorGradient: {ex.Message}");
            }

            // Enregistrez le classeur pour démontrer l'effet
            workbook.Save("SetTwoColorGradientWithTransparencyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



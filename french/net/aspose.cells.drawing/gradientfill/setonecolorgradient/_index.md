---
title: "GradientFill.SetOneColorGradient"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GradientFill. Définit le remplissage spécifié comme un dégradé à une couleur. S'applique uniquement à Excel 2007"
type: docs
url: /fr/net/aspose.cells.drawing/gradientfill/setonecolorgradient/
---
## GradientFill.SetOneColorGradient method

Définit le remplissage spécifié comme un dégradé à une couleur. S'applique uniquement à Excel 2007.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| color | Color | Une couleur de dégradé. |
| degré | Double | Le degré du dégradé. Peut être une valeur de 0.0 (sombre) à 1.0 (clair). |
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

    public class GradientFillMethodSetOneColorGradientWithColorDoubleGradientStyleTyInt32Demo
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

                // Appeler SetOneColorGradient avec des paramètres réalistes
                gradientFill.SetOneColorGradient(
                    Color.Green,        // color
                    0.7,                // degree (70% intensity)
                    GradientStyleType.DiagonalUp,  // style
                    1);                 // variant

                Console.WriteLine("SetOneColorGradient method called successfully with parameters (Green, 0.7, DiagonalUp, 1)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOneColorGradient: {ex.Message}");
            }

            // Enregistrez le classeur pour démontrer l'effet
            workbook.Save("SetOneColorGradientDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



---
title: "Style.GetTwoColorGradient"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Style. Obtient le paramètre de dégradé à deux couleurs"
type: docs
url: /fr/net/aspose.cells/style/gettwocolorgradient/
---
## Style.GetTwoColorGradient method

Obtenir le paramètre de dégradé bicolore.

```csharp
[Obsolete("Use Style.GetTwoColorGradientSetting() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GetTwoColorGradient(out Color color1, out Color color2, 
    out GradientStyleType gradientStyleType, out int variant)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| color1 | Color& | Une couleur de dégradé. |
| color2 | Color& | Deux couleurs de dégradé. |
| gradientStyleType | GradientStyleType& | Style d’ombrage du dégradé. |
| variant | Int32& | La variante du dégradé. |

### Remarques

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode Style.GetTwoColorGradientSetting(). Cette propriété sera supprimée 12 mois plus tard, depuis décembre 2022. Aspose s’excuse pour tout inconvénient que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class StyleMethodGetTwoColorGradientWithColorColorGradientStyleTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un style et définir un dégradé à deux couleurs
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 1);

            // Appliquer le style à une cellule
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Two Color Gradient Demo");

            // Préparer les variables pour obtenir les paramètres du dégradé
            Color color1 = Color.Empty;
            Color color2 = Color.Empty;
            GradientStyleType gradientStyle = GradientStyleType.Horizontal;
            int variant = 0;

            try
            {
                // Appeler la méthode GetTwoColorGradient
#pragma warning disable CS0618 // Type or member is obsolete
                style.GetTwoColorGradient(out color1, out color2, out gradientStyle, out variant);
#pragma warning restore CS0618 // Type or member is obsolete

                // Afficher les paramètres du dégradé récupérés
                Console.WriteLine("Gradient Settings:");
                Console.WriteLine($"Color1: {color1}");
                Console.WriteLine($"Color2: {color2}");
                Console.WriteLine($"Gradient Style: {gradientStyle}");
                Console.WriteLine($"Variant: {variant}");

                // Enregistrez le classeur
                workbook.Save("StyleMethodGetTwoColorGradientDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTwoColorGradient method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



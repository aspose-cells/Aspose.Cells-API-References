---
title: "Style.SetTwoColorGradient"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Style. Définit le remplissage spécifié en un dégradé bicolore"
type: docs
url: /fr/net/aspose.cells/style/settwocolorgradient/
---
## Style.SetTwoColorGradient method

Définit le remplissage spécifié en un dégradé bicolore.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType gradientStyleType, 
    int variant)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| color1 | Color | Une couleur de dégradé. |
| color2 | Color | Deux couleurs de dégradé. |
| gradientStyleType | GradientStyleType | Style d’ombrage du dégradé. |
| variant | Int32 | La variante du dégradé. Peut être une valeur de 1 à 4, correspondant à l'une des quatre variantes de l'onglet Dégradé dans la boîte de dialogue Effets de remplissage. Si le style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2. |

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez un objet de style
            Style style = workbook.CreateStyle();

            // Définissez un dégradé bicolore pour le style
            style.SetTwoColorGradient(Color.Green, Color.Red, GradientStyleType.Vertical, 1);

            // Appliquer le style à une cellule
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Gradient Style Demo");

            // Vérifiez les paramètres du dégradé
            Color color1, color2;
            GradientStyleType gradientStyle;
            int variant;
            style.GetTwoColorGradient(out color1, out color2, out gradientStyle, out variant);

            Console.WriteLine("Color1: " + color1);
            Console.WriteLine("Color2: " + color2);
            Console.WriteLine("Gradient Style: " + gradientStyle);
            Console.WriteLine("Variant: " + variant);

            // Enregistrez le classeur
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



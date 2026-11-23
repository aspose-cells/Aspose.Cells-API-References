---
title: "Workbook.GetMatchingColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Trouve la couleur la plus proche dans la palette actuelle"
type: docs
url: /fr/net/aspose.cells/workbook/getmatchingcolor/
---
## Workbook.GetMatchingColor method

Trouve la couleur correspondante la plus proche dans la palette actuelle.

```csharp
public Color GetMatchingColor(Color rawColor)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rawColor | Color | Couleur brute. |

### Valeur de retour

Meilleure couleur correspondante.

### Remarques

Il n'y a que 56 couleurs dans la palette de couleurs d'Excel 97-2003. Si la couleur n'est pas dans la palette, une couleur similaire sera définie.

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetMatchingColorWithColorDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Vérifiez si la couleur existe dans la palette
            Console.WriteLine("Is Red in palette: " + workbook.IsColorInPalette(Color.Red));
            Color testColor = Color.FromArgb(255, 123, 123, 123);
            Console.WriteLine("Is custom color in palette: " + workbook.IsColorInPalette(testColor));

            // Obtenir la couleur correspondante de la palette
            Color matchedColor = workbook.GetMatchingColor(testColor);
            Console.WriteLine($"Original color: R={testColor.R}, G={testColor.G}, B={testColor.B}");
            Console.WriteLine($"Matched color: R={matchedColor.R}, G={matchedColor.G}, B={matchedColor.B}");

            // Créez un thème personnalisé
            Color[] themeColors = new Color[12];
            for (int i = 0; i < themeColors.Length; i++)
            {
                themeColors[i] = Color.FromArgb(255, 128 + i, 128 + i, 128 + i);
            }
            workbook.CustomTheme("CustomTheme", themeColors);

            // Obtenez la couleur du thème
            Color themeColor = workbook.GetThemeColor(ThemeColorType.FollowedHyperlink);
            Console.WriteLine($"Theme color: R={themeColor.R}, G={themeColor.G}, B={themeColor.B}");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



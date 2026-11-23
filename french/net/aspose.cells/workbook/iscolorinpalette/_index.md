---
title: "Workbook.IsColorInPalette"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Vérifie si une couleur se trouve dans la palette du classeur"
type: docs
url: /fr/net/aspose.cells/workbook/iscolorinpalette/
---
## Workbook.IsColorInPalette method

Vérifie si une couleur se trouve dans la palette de la feuille de calcul.

```csharp
public bool IsColorInPalette(Color color)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| color | Color | Structure Color. |

### Valeur de retour

Renvoie true si cette couleur est dans la palette. Sinon, renvoie false

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodIsColorInPaletteWithColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Vérifier si la couleur standard existe dans la palette
            bool isRedInPalette = workbook.IsColorInPalette(Color.Red);
            Console.WriteLine("Is Red in palette: " + isRedInPalette);
            
            // Vérifier si la couleur personnalisée existe dans la palette
            Color customColor = Color.FromArgb(255, 123, 123, 123);
            bool isCustomInPalette = workbook.IsColorInPalette(customColor);
            Console.WriteLine("Is custom color in palette: " + isCustomInPalette);
            
            // Obtenir la couleur correspondante de la palette
            Color matchedColor = workbook.GetMatchingColor(customColor);
            Console.WriteLine("Matched color R value: " + matchedColor.R);
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



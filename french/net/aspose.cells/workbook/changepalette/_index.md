---
title: "Workbook.ChangePalette"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Modifie la palette du tableau dans l'index spécifié"
type: docs
url: /fr/net/aspose.cells/workbook/changepalette/
---
## Workbook.ChangePalette method

Modifie la palette de la feuille de calcul à l'index spécifié.

```csharp
public void ChangePalette(Color color, int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| color | Color | Structure Color. |
| indice | Int32 | Index de la palette, 0 - 55. |

### Remarques

La palette comporte 56 entrées, chacune représentée par une valeur RVB.

Si vous définissez une couleur qui n'est pas dans la palette, elle ne prendra pas effet.

Donc, si vous souhaitez définir une couleur personnalisée, veuillez d'abord modifier la palette.

Voici la palette de couleurs standard.

| **Color** | **Red** | **Vert** | **Bleu** |
| --- | --- | --- | --- |
| Noir | 0 | 0 | 0 |
| Blanc | 255 | 255 | 255 |
| Rouge | 255 | 0 | 0 |
| Citron vert | 0 | 255 | 0 |
| Bleu | 0 | 0 | 255 |
| Jaune | 255 | 255 | 0 |
| Magenta | 255 | 0 | 255 |
| Cyan | 0 | 255 | 255 |
| Marron | 128 | 0 | 0 |
| Vert | 0 | 128 | 0 |
| Marine | 0 | 0 | 128 |
| Olive | 128 | 128 | 0 |
| Violet | 128 | 0 | 128 |
| Sarcelle | 0 | 128 | 128 |
| Argent | 192 | 192 | 192 |
| Gris | 128 | 128 | 128 |
| Color17 | 153 | 153 | 255 |
| Color18 | 153 | 51 | 102 |
| Color19 | 255 | 255 | 204 |
| Color20 | 204 | 255 | 255 |
| Color21 | 102 | 0 | 102 |
| Color22 | 255 | 128 | 128 |
| Color23 | 0 | 102 | 204 |
| Color24 | 204 | 204 | 255 |
| Color25 | 0 | 0 | 128 |
| Color26 | 255 | 0 | 255 |
| Color27 | 255 | 255 | 0 |
| Color28 | 0 | 255 | 255 |
| Color29 | 128 | 0 | 128 |
| Color30 | 128 | 0 | 0 |
| Color31 | 0 | 128 | 128 |
| Color32 | 0 | 0 | 255 |
| Color33 | 0 | 204 | 255 |
| Color34 | 204 | 255 | 255 |
| Color35 | 204 | 255 | 204 |
| Color36 | 255 | 255 | 153 |
| Color37 | 153 | 204 | 255 |
| Color38 | 255 | 153 | 204 |
| Color39 | 204 | 153 | 255 |
| Color40 | 255 | 204 | 153 |
| Color41 | 51 | 102 | 255 |
| Color42 | 51 | 204 | 204 |
| Color43 | 153 | 204 | 0 |
| Color44 | 255 | 204 | 0 |
| Color45 | 255 | 153 | 0 |
| Color46 | 255 | 102 | 0 |
| Color47 | 102 | 102 | 153 |
| Color48 | 150 | 150 | 150 |
| Color49 | 0 | 51 | 102 |
| Color50 | 51 | 153 | 102 |
| Color51 | 0 | 51 | 0 |
| Color52 | 51 | 51 | 0 |
| Color53 | 153 | 51 | 0 |
| Color54 | 153 | 51 | 102 |
| Color55 | 51 | 51 | 153 |
| Color56 | 51 | 51 | 51 |

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodChangePaletteWithColorInt32Demo
    {
        public static void Run()
        {
            // Créer une instance de classe Workbook
            Workbook workbook = new Workbook();
            
            // Modifier la couleur de la palette à l'index 55
            Color newColor = Color.FromArgb(255, 250, 223);
            workbook.ChangePalette(newColor, 55);

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer un style avec la couleur de palette modifiée
            Style style = workbook.CreateStyle();
            style.ForegroundColor = newColor;
            style.Pattern = BackgroundType.Solid;

            // Appliquer le style à une cellule
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Palette Color Demo");
            cell.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("ChangePaletteDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



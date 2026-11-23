---
title: "Énumération PresetWordArtStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.PresetWordArtStyle. Représente les styles WordArt prédéfinis"
type: docs
url: /fr/net/aspose.cells.drawing/presetwordartstyle/
---
## PresetWordArtStyle enumeration

Représente les styles WordArt prédéfinis.

```csharp
public enum PresetWordArtStyle
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| WordArtStyle1 | `1` | Remplissage - Noir, Texte 1, Ombre |
| WordArtStyle2 | `2` | Remplissage - Bleu, Accent 1, Ombre |
| WordArtStyle3 | `3` | Remplissage - Orange, Accent 2, Contour - Accent 2 |
| WordArtStyle4 | `4` | Remplissage - Blanc, Contour - Accent 1, Ombre |
| WordArtStyle5 | `5` | Remplissage - Or, Accent 4, Biseau doux |
| WordArtStyle6 | `6` | Remplissage en dégradé - Gris |
| WordArtStyle7 | `7` | Remplissage en dégradé - Bleu, Accent 1, Réflexion |
| WordArtStyle8 | `8` | Remplissage en dégradé - Or, Accent 4, Contour - Accent 4 |
| WordArtStyle9 | `9` | Remplissage - Blanc, Contour - Accent 1, Lueur - Accent 1 |
| WordArtStyle10 | `10` | Remplissage - Gris-50 %, Accent 3, Biseau net |
| WordArtStyle11 | `11` | Remplissage - Noir, Texte 1, Contour - Arrière-plan 1, Ombre dure - Arrière-plan 1 |
| WordArtStyle12 | `12` | Remplissage - Noir, Texte 1, Contour - Arrière-plan 1, Ombre dure - Accent 1 |
| WordArtStyle13 | `13` | Remplissage - Bleu, Accent 1, Contour - Arrière-plan 1, Ombre dure - Accent 1 |
| WordArtStyle14 | `14` | Remplissage - Blanc, Contour - Accent 2, Ombre dure - Accent 2 |
| WordArtStyle15 | `15` | Remplissage - Gris-25%, Arrière-plan 2, Ombre interne |
| WordArtStyle16 | `16` | Remplissage de motif - Blanc, Texte 2, Diagonale sombre ascendante, Ombre |
| WordArtStyle17 | `17` | Remplissage de motif - Gris-50%, Accent 3, Horizontal étroit, Ombre interne |
| WordArtStyle18 | `18` | Remplissage - Bleu, Accent 1, 50%, Ombre dure - Accent 1 |
| WordArtStyle19 | `19` | Remplissage de motif - Bleu, Accent 1, Diagonale claire descendante, Contour - Accent 1 |
| WordArtStyle20 | `20` | Remplissage de motif - Bleu-gris, Texte 2, Diagonale sombre ascendante, Ombre dure - Texte 2 |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PresetWordArtStyleDemo
    {
        public static void PresetWordArtStyleExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la collection de formes de la feuille de calcul
            ShapeCollection shapes = worksheet.Shapes;
            
            // Ajouter une forme WordArt avec un style prédéfini spécifique
            // Paramètres : style, text, upperLeftRow, top, upperLeftColumn, left, height, width
            Shape wordArt = shapes.AddWordArt(PresetWordArtStyle.WordArtStyle2, "Hello Aspose!", 1, 0, 1, 0, 100, 400);
            
            // Enregistrez le classeur
            workbook.Save("PresetWordArtStyleExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



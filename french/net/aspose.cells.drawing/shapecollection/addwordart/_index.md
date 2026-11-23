---
title: "ShapeCollection.AddWordArt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute un WordArt prédéfini depuis Excel 2007."
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addwordart/
---
## ShapeCollection.AddWordArt method

Ajoute WordArt prédéfini depuis Excel 2007.s

```csharp
public Shape AddWordArt(PresetWordArtStyle style, string text, int topRow, int top, int leftColumn, 
    int left, int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| style | PresetWordArtStyle | Le style WordArt prédéfini. |
| texte | String | Le texte. |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| haut | Int32 | Représente le décalage vertical de la forme depuis sa ligne gauche, en unité de pixel. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| gauche | Int32 | Représente le décalage horizontal de la forme par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | Int32 | Représente la hauteur de la forme, en unités de pixel. |
| largeur | Int32 | Représente la largeur de la forme, en unité de pixel. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddWordArtWithPresetWordArtStyleStringInt32IDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir la collection de formes
            ShapeCollection shapes = worksheet.Shapes;

            // Ajouter un WordArt avec des paramètres spécifiés
            Shape wordArt = shapes.AddWordArt(
                PresetWordArtStyle.WordArtStyle1, 
                "Sample WordArt", 
                10,  // left
                10,  // top
                200, // width
                50,  // height
                100, // rotation
                200  // z-order
            );

            // Enregistrez le classeur
            workbook.Save("WordArtDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../../shape/)
* enum [PresetWordArtStyle](../../presetwordartstyle/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



---
title: "ShapeCollection.AddLabel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute un Label à la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addlabel/
---
## ShapeCollection.AddLabel method

Ajoute une étiquette à la feuille de calcul.

```csharp
public Label AddLabel(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| haut | Int32 | Représente le décalage vertical du Label par rapport à sa ligne de gauche, en unité de pixel. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| gauche | Int32 | Représente le décalage horizontal du Label par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | Int32 | Représente la hauteur du Label, en unité de pixel. |
| largeur | Int32 | Représente la largeur du Label, en unité de pixel. |

### Valeur de retour

Un objet Label.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLabelWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir la collection de formes
            ShapeCollection shapes = worksheet.Shapes;

            // Ajouter un label à la feuille de calcul
            Label label = shapes.AddLabel(1, 0, 1, 0, 100, 50);
            label.Text = "Sample Label";

            // Enregistrez le classeur
            workbook.Save("AddLabelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



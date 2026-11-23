---
title: "ShapeCollection.AddButton"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute un Button à la feuille de calcul."
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addbutton/
---
## ShapeCollection.AddButton method

Ajoute un Button à la feuille de calcul.

```csharp
public Button AddButton(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| haut | Int32 | Représente le décalage vertical de Button par rapport à sa ligne de gauche, en unité de pixel. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| gauche | Int32 | Représente le décalage horizontal de Button par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | Int32 | Représente la hauteur de Button, en unité de pixel. |
| largeur | Int32 | Représente la largeur de Button, en unité de pixel. |

### Valeur de retour

Un objet Button.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddButtonWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un bouton en utilisant les paramètres spécifiés
            Aspose.Cells.Drawing.Button button = worksheet.Shapes.AddButton(1, 0, 1, 0, 100, 50);
            button.Text = "Click Me";

            // Enregistrez le classeur
            workbook.Save("ButtonDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Button](../../button/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



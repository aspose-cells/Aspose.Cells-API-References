---
title: "ShapeCollection.AddCheckBox"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute une case à cocher à la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addcheckbox/
---
## ShapeCollection.AddCheckBox method

Ajoute une case à cocher à la feuille de calcul.

```csharp
public CheckBox AddCheckBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| haut | Int32 | Représente le décalage vertical de la case à cocher par rapport à sa ligne supérieure, en unité de pixel. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| gauche | Int32 | Représente le décalage horizontal de la zone de texte par rapport à sa colonne gauche, en pixels. |
| hauteur | Int32 | Hauteur de la zone de texte, en unité de pixel. |
| largeur | Int32 | Largeur de la zone de texte, en unité de pixel. |

### Valeur de retour

L'index du nouvel objet CheckBox.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddCheckBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir la collection de formes
            ShapeCollection shapes = worksheet.Shapes;

            // Ajouter une CheckBox en utilisant les paramètres spécifiés
            Aspose.Cells.Drawing.CheckBox checkBox = shapes.AddCheckBox(1, 0, 1, 0, 100, 50);

            // Enregistrez le classeur
            workbook.Save("CheckBoxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CheckBox](../../checkbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



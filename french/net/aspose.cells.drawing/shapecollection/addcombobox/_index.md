---
title: "ShapeCollection.AddComboBox"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute une ComboBox à la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addcombobox/
---
## ShapeCollection.AddComboBox method

Ajoute un ComboBox à la feuille de calcul.

```csharp
public ComboBox AddComboBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| haut | Int32 | Représente le décalage vertical de la ComboBox par rapport à sa ligne de gauche, en unité de pixel. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| gauche | Int32 | Représente le décalage horizontal de la ComboBox par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | Int32 | Représente la hauteur de la ComboBox, en unité de pixel. |
| largeur | Int32 | Représente la largeur de la ComboBox, en unité de pixel. |

### Valeur de retour

Un objet ComboBox.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddComboBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir la collection de formes
            ShapeCollection shapes = worksheet.Shapes;

            // Ajoutez une combo box avec les paramètres spécifiés
            Aspose.Cells.Drawing.ComboBox comboBox = shapes.AddComboBox(1, 0, 1, 0, 100, 50);

            // Ajoutez des éléments à la combo box en définissant les valeurs des cellules
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Définir la plage d'entrée pour la boîte combinée
            comboBox.InputRange = "A1:A3";
            comboBox.DropDownLines = 3;

            // Enregistrez le classeur
            workbook.Save("AddComboBoxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ComboBox](../../combobox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



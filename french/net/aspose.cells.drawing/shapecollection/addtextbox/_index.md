---
title: "ShapeCollection.AddTextBox"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute une zone de texte à la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addtextbox/
---
## ShapeCollection.AddTextBox method

Ajoute une zone de texte à la feuille de calcul.

```csharp
public TextBox AddTextBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| haut | Int32 | Représente le décalage vertical de la zone de texte par rapport à sa ligne supérieure, en pixels. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| gauche | Int32 | Représente le décalage horizontal de la zone de texte par rapport à sa colonne gauche, en pixels. |
| hauteur | Int32 | Représente la hauteur de la zone de texte, en pixels. |
| largeur | Int32 | Représente la largeur de la zone de texte, en pixels. |

### Valeur de retour

Un objet [`TextBox`](../../textbox/).

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir la collection de formes
            ShapeCollection shapes = worksheet.Shapes;

            // Ajouter une zone de texte avec la position et la taille spécifiées
            TextBox textBox = shapes.AddTextBox(1, 0, 1, 0, 100, 50);
            textBox.Text = "Sample TextBox";

            // Enregistrez le classeur
            workbook.Save("TextBoxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



---
title: "ShapeCollection.AddRadioButton"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute un RadioButton à la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addradiobutton/
---
## ShapeCollection.AddRadioButton method

Ajoute un RadioButton à la feuille de calcul.

```csharp
public RadioButton AddRadioButton(int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| haut | Int32 | Représente le décalage vertical du RadioButton depuis sa ligne gauche, en unité de pixel. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| gauche | Int32 | Représente le décalage horizontal du RadioButton par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | Int32 | Représente la hauteur du RadioButton, en unité de pixel. |
| largeur | Int32 | Représente la largeur du RadioButton, en unité de pixel. |

### Valeur de retour

Un objet RadioButton.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddRadioButtonWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un bouton radio à la feuille de calcul
            Aspose.Cells.Drawing.RadioButton radioButton = worksheet.Shapes.AddRadioButton(1, 0, 1, 0, 100, 50);
            radioButton.Text = "Option 1";

            // Enregistrez le classeur
            workbook.Save("RadioButtonDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [RadioButton](../../radiobutton/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



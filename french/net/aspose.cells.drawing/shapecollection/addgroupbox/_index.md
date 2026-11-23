---
title: "ShapeCollection.AddGroupBox"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute un GroupBox à la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addgroupbox/
---
## ShapeCollection.AddGroupBox method

Ajoute une GroupBox à la feuille de calcul.

```csharp
public GroupBox AddGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| haut | Int32 | Représente le décalage vertical du GroupBox depuis sa ligne de gauche, en unité de pixel. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| gauche | Int32 | Représente le décalage horizontal du GroupBox depuis sa colonne de gauche, en unité de pixel. |
| hauteur | Int32 | Représente la hauteur du GroupBox, en unité de pixel. |
| largeur | Int32 | Représente la largeur du GroupBox, en unité de pixel. |

### Valeur de retour

Un objet GroupBox.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddGroupBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un group box à la feuille de calcul
            ShapeCollection shapes = worksheet.Shapes;
            Aspose.Cells.Drawing.GroupBox groupBox = shapes.AddGroupBox(1, 0, 1, 0, 100, 50);

            // Enregistrez le classeur
            workbook.Save("GroupBoxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [GroupBox](../../groupbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



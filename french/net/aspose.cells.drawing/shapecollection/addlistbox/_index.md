---
title: "ShapeCollection.AddListBox"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute une ListBox à la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addlistbox/
---
## ShapeCollection.AddListBox method

Ajoute une ListBox à la feuille de calcul.

```csharp
public ListBox AddListBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| haut | Int32 | Représente le décalage vertical de la ListBox par rapport à sa ligne de gauche, en unité de pixel. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| gauche | Int32 | Représente le décalage horizontal de la ListBox par rapport à sa colonne de gauche, en unité de pixel. |
| hauteur | Int32 | Représente la hauteur de la ListBox, en unité de pixel. |
| largeur | Int32 | Représente la largeur de la ListBox, en unité de pixel. |

### Valeur de retour

Un objet ListBox.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddListBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de liste à la feuille de calcul
            Aspose.Cells.Drawing.ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 0, 100, 50);

            // Ajouter des éléments à la zone de liste
            listBox.SetInputRange("A1:A3", false, false);
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Enregistrez le classeur
            workbook.Save("ListBoxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListBox](../../listbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



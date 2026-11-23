---
title: "ShapeCollection.AddSpinner"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Ajoute un Spinner à la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/addspinner/
---
## ShapeCollection.AddSpinner method

Ajoute un Spinner à la feuille de calcul.

```csharp
public Spinner AddSpinner(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Indice de la ligne supérieure gauche. |
| haut | Int32 | Représente le décalage vertical du Spinner depuis sa ligne de gauche, en pixels. |
| leftColumn | Int32 | Indice de la colonne supérieure gauche. |
| gauche | Int32 | Représente le décalage horizontal du Spinner depuis sa colonne de gauche, en pixels. |
| hauteur | Int32 | Représente la hauteur du Spinner, en pixels. |
| largeur | Int32 | Représente la largeur du Spinner, en pixels. |

### Valeur de retour

Un objet Spinner.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddSpinnerWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un spinner à la feuille de calcul
            Aspose.Cells.Drawing.Spinner spinner = (Aspose.Cells.Drawing.Spinner)worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 50);

            // Définir les propriétés du Spinner
            spinner.LinkedCell = "A1";
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 1;

            // Enregistrez le classeur
            workbook.Save("AddSpinnerDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Spinner](../../spinner/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



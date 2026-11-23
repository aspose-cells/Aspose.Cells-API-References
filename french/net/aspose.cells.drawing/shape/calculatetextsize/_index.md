---
title: "Shape.CalculateTextSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Recalculer la zone de texte"
type: docs
url: /fr/net/aspose.cells.drawing/shape/calculatetextsize/
---
## Shape.CalculateTextSize method

Recalculer la zone de texte

```csharp
public int[] CalculateTextSize()
```

### Valeur de retour

Taille du texte dans un tableau (largeur et hauteur).

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodCalculateTextSizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un texte d'exemple à la cellule A1
            worksheet.Cells["A1"].PutValue("Sample Text for Size Calculation");

            // Créer une forme rectangulaire avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Définir le texte pour la forme
            shape.Text = "This is a test string to calculate text size";

            // Calculer la taille du texte
            int[] size = shape.CalculateTextSize();

            // Afficher les résultats
            Console.WriteLine($"Calculated text size - Width: {size[0]}, Height: {size[1]}");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



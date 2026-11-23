---
title: "Shape.GetActualBox"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Obtient la position et la taille réelles de la forme après application de la rotation, du retournement, etc."
type: docs
url: /fr/net/aspose.cells.drawing/shape/getactualbox/
---
## Shape.GetActualBox method

Obtenir la position et la taille réelles de la forme (après application de la rotation, du retournement, etc.)

```csharp
public float[] GetActualBox()
```

### Valeur de retour

Renvoie la position et la taille dans l'ordre x, y, l, h

### Remarques

Remarque: l'interface n'est pas entièrement fonctionnelle, en particulier les informations de localisation ne sont pas correctes. Il est recommandé de ne pas utiliser cette interface tant que la fonction n'est pas terminée.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetActualBoxDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape rectangle = worksheet.Shapes.AddRectangle(10, 10, 100, 80, 0, 0);

            // Obtenez les dimensions réelles de la boîte de la forme
            float[] box = rectangle.GetActualBox();

            // Affichez les dimensions de la boîte
            Console.WriteLine("Actual Box Dimensions:");
            Console.WriteLine($"Left: {box[0]}");
            Console.WriteLine($"Top: {box[1]}");
            Console.WriteLine($"Right: {box[2]}");
            Console.WriteLine($"Bottom: {box[3]}");

            // Enregistrez le classeur
            workbook.Save("ShapeGetActualBoxDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



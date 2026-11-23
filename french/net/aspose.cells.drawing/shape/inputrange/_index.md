---
title: "Shape.InputRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient ou définit la plage de la feuille de calcul utilisée pour remplir la boîte combinée spécifiée"
type: docs
url: /fr/net/aspose.cells.drawing/shape/inputrange/
---
## Shape.InputRange property

Obtient ou définit la plage de feuille de calcul utilisée pour remplir la zone combinée spécifiée.

```csharp
public string InputRange { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyInputRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Value 1");
            worksheet.Cells["A2"].PutValue("Value 2");
            worksheet.Cells["A3"].PutValue("Value 3");
            worksheet.Cells["A4"].PutValue("Value 4");
            worksheet.Cells["A5"].PutValue("Value 5");

            // Ajouter une forme (rectangle)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Définir la plage d'entrée pour la forme
            shape.InputRange = "$A$1:$A$5";

            // Vérifier et modifier la plage d'entrée si nécessaire
            if (shape.InputRange.Equals("$A$1:$A$5"))
            {
                shape.InputRange = "$B$1:$B$5";
                Console.WriteLine("Input range changed to: " + shape.InputRange);
            }
            else
            {
                Console.WriteLine("Current input range: " + shape.InputRange);
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



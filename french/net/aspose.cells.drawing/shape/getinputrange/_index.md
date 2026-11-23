---
title: "Shape.GetInputRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Obtient la plage utilisée pour remplir le contrôle"
type: docs
url: /fr/net/aspose.cells.drawing/shape/getinputrange/
---
## Shape.GetInputRange method

Obtient la plage utilisée pour remplir le contrôle.

```csharp
public string GetInputRange(bool isR1C1, bool isLocal)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | Boolean | Indique si la formule doit être formatée selon la locale. |

### Valeur de retour

La plage utilisée pour remplir le contrôle.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetInputRangeWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Input 1");
            worksheet.Cells["A2"].PutValue("Input 2");
            worksheet.Cells["A3"].PutValue("Input 3");

            // Ajouter une forme de zone de liste
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 0, 0);
            Shape shape = listBox;

            // Définir la plage d'entrée pour la zone de liste
            shape.SetInputRange("$A$1:$A$3", false, false);

            // Obtenir la plage d'entrée
            string range = shape.GetInputRange(false, true);
            Console.WriteLine("Shape input range: " + range);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



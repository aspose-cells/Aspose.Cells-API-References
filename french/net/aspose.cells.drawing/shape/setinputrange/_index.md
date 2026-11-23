---
title: "Shape.SetInputRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Définit la plage utilisée pour remplir le contrôle"
type: docs
url: /fr/net/aspose.cells.drawing/shape/setinputrange/
---
## Shape.SetInputRange method

Définit la plage utilisée pour remplir le contrôle.

```csharp
public void SetInputRange(string formula, bool isR1C1, bool isLocal)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formule | String | La plage utilisée pour remplir le contrôle. |
| isR1C1 | Boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | Boolean | Indique si la formule doit être formatée selon la locale. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetInputRangeWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un objet classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple aux cellules A1:A10
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;
            }

            // Ajouter une forme de zone de liste
            Aspose.Cells.Drawing.Shape listBox = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);

            // Définir la plage d'entrée pour la zone de liste (en utilisant les paramètres String, Boolean, Boolean)
            listBox.SetInputRange("$A$1:$A$6", false, false);

            // Définir la cellule liée pour la zone de liste
            listBox.SetLinkedCell("$A$12", false, true);

            // Enregistrez le classeur
            workbook.Save("SetInputRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



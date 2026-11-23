---
title: "Shape.UpdateSelectedValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Mettre à jour la valeur sélectionnée par la valeur de la cellule liée"
type: docs
url: /fr/net/aspose.cells.drawing/shape/updateselectedvalue/
---
## Shape.UpdateSelectedValue method

Met à jour la valeur sélectionnée avec la valeur de la cellule liée.

```csharp
public void UpdateSelectedValue()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodUpdateSelectedValueDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;
            }

            // Créer une forme ListBox
            Shape listBoxShape = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);
            
            // Définir la plage d'entrée et la cellule liée
            listBoxShape.SetInputRange("$A$1:$A$6", false, false);
            listBoxShape.SetLinkedCell("$A$12", false, true);

            // Obtenir l'objet ListBox
            ListBox listBox = (ListBox)listBoxShape;

            // Définir la valeur initiale dans la cellule liée et mettre à jour la sélection
            worksheet.Cells["A12"].Value = 3;
            listBoxShape.UpdateSelectedValue();

            // Vérifier la sélection
            if (listBox.IsSelected(2))
            {
                Console.WriteLine("Option 3 is selected");
            }

            // Modifier la valeur et mettre à jour la sélection à nouveau
            worksheet.Cells["A12"].Value = 4;
            listBoxShape.UpdateSelectedValue();

            if (listBox.IsSelected(3))
            {
                Console.WriteLine("Option 4 is selected");
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



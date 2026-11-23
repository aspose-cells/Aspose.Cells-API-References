---
title: "ShapeCollection.UpdateSelectedValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapeCollection. Met à jour la valeur sélectionnée par la valeur de la cellule liée ou de la plage de la forme"
type: docs
url: /fr/net/aspose.cells.drawing/shapecollection/updateselectedvalue/
---
## ShapeCollection.UpdateSelectedValue method

Met à jour la valeur sélectionnée avec la valeur de la cellule liée ou de la plage de la forme.

```csharp
public void UpdateSelectedValue()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodUpdateSelectedValueDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme (liste déroulante) à la feuille de calcul
            Aspose.Cells.Drawing.ListBox listBox = (Aspose.Cells.Drawing.ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 3, 20);
            
            // Définir les éléments de la liste et la valeur sélectionnée
            listBox.SetInputRange("A1:A3", false, false);
            listBox.SelectedIndex = 1;
            
            // Mettre à jour la valeur sélectionnée dans la forme
            worksheet.Shapes.UpdateSelectedValue();
            
            // Enregistrez le classeur
            workbook.Save("ShapeCollectionUpdateSelectedValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



---
title: "ListBox.SelectionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListBox. Obtient ou définit le mode de sélection de la list box spécifiée"
type: docs
url: /fr/net/aspose.cells.drawing/listbox/selectiontype/
---
## ListBox.SelectionType property

Obtient ou définit le mode de sélection de la zone de liste spécifiée.

```csharp
public SelectionType SelectionType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertySelectionTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour la list box
            sheet.Cells["A1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Finance");
            sheet.Cells["A3"].PutValue("MIS");
            sheet.Cells["A4"].PutValue("R&D");

            // Ajouter une list box
            ListBox listBox = sheet.Shapes.AddListBox(1, 0, 2, 0, 100, 80);
            
            // Définir les propriétés de la list box
            listBox.InputRange = "A1:A4";
            listBox.LinkedCell = "B1";
            
            // Démontrer la propriété SelectionType
            listBox.SelectionType = SelectionType.Single; // Only single selection allowed
            listBox.SelectedIndex = 1; // Select "Finance"

            // Enregistrez le classeur
            workbook.Save("ListBoxSelectionTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SelectionType](../../selectiontype/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



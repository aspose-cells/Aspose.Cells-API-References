---
title: "ListBox.IsSelected"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ListBox. Indique si l'élément est sélectionné"
type: docs
url: /fr/net/aspose.cells.drawing/listbox/isselected/
---
## ListBox.IsSelected method

Indique si l'élément est sélectionné.

```csharp
public bool IsSelected(int itemIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| itemIndex | Int32 | L'index de l'élément. |

### Valeur de retour

si l'élément est sélectionné.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxMethodIsSelectedWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de liste à la feuille de calcul
            ListBox listBox = worksheet.Shapes.AddListBox(0, 0, 100, 100, 200, 200);

            // Définir les éléments de la liste via la plage de cellules liée
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            listBox.LinkedCell = "A1:A3";

            // Sélectionnez un élément
            listBox.SelectedIndex = 0;

            // Vérifiez l'état de la sélection en utilisant IsSelected avec le paramètre Int32
            Console.WriteLine("Item 0 selected: " + listBox.IsSelected(0));
            Console.WriteLine("Item 1 selected: " + listBox.IsSelected(1));
            Console.WriteLine("Item 2 selected: " + listBox.IsSelected(2));
        }
    }
}
```

### Voir aussi

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



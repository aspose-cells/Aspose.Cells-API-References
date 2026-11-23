---
title: "ListBox.PageChange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListBox. Spécifie la quantité de changement de la valeur du contrôle lorsque l'utilisateur clique sur la zone de défilement page précédente ou page suivante"
type: docs
url: /fr/net/aspose.cells.drawing/listbox/pagechange/
---
## ListBox.PageChange property

Spécifie la quantité par laquelle la valeur du contrôle est modifiée lorsque l'utilisateur clique sur la zone de défilement page précédente ou page suivante.

```csharp
public int PageChange { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertyPageChangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme ListBox
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(1, 0, 1, 0, 100, 100);

            // Définir certains éléments pour la ListBox
            listBox.SetInputRange("A1:A5", false, false);
            
            // Définir la propriété PageChange
            listBox.PageChange = 2;

            // Enregistrez le classeur
            workbook.Save("ListBoxPageChangeDemo.xlsx");

            // Afficher la valeur de PageChange
            Console.WriteLine("ListBox PageChange value: " + listBox.PageChange);
        }
    }
}
```

### Voir aussi

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



---
title: "ListBox.SelectedCells"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ListBox. Obtient les cellules sélectionnées. Retourne null si la plage d'entrée n'est pas définie ou aucun élément n'est sélectionné"
type: docs
url: /fr/net/aspose.cells.drawing/listbox/selectedcells/
---
## ListBox.SelectedCells property

Obtient les cellules sélectionnées. Retourne null si la plage d'entrée n'est pas définie ou aucun élément n'est sélectionné

```csharp
public Cell[] SelectedCells { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ListBoxPropertySelectedCellsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir des données d'exemple pour les éléments de ListBox
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");

            // Créer une ListBox et la lier à la plage de données
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(7, 0, 100, 150, 5, 1);
            listBox.InputRange = "A1:A5";
            listBox.SelectionType = SelectionType.Multi;

            // Sélectionner plusieurs éléments en utilisant des index à base zéro
            listBox.SelectedItem(0, true);
            listBox.SelectedItem(2, true);

            // Récupérer et afficher les cellules sélectionnées
            Cell[] selectedCells = listBox.SelectedCells;
            Console.WriteLine("Selected Cells Count: " + selectedCells.Length);
            
            // Modifier les cellules sélectionnées pour démontrer l'accès
            foreach (Cell cell in selectedCells)
            {
                Console.WriteLine("Selected Cell Address: " + cell.Name);
                cell.PutValue("[SELECTED] " + cell.StringValue);
            }

            workbook.Save("ListBoxSelectedCellsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../../../aspose.cells/cell/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



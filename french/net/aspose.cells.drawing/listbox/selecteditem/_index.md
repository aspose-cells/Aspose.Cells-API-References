---
title: "ListBox.SelectedItem"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ListBox. Définit si l'élément est sélectionné"
type: docs
url: /fr/net/aspose.cells.drawing/listbox/selecteditem/
---
## ListBox.SelectedItem method

Définit si l'élément est sélectionné

```csharp
public void SelectedItem(int itemIndex, bool isSelected)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| itemIndex | Int32 | L'index de l'élément |
| isSelected | Boolean | Indique si l'élément est sélectionné. True signifie que cet élément doit être sélectionné. False signifie que cet élément doit être désélectionné. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ListBoxMethodSelectedItemWithInt32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir les éléments de la liste
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i, 0].Value = $"Item {i + 1}";
            }

            // Créer une list box
            ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 150, 100) as ListBox;
            listBox.InputRange = "A1:A5";
            listBox.SelectionType = SelectionType.Multi;

            try
            {
                // Sélectionner et désélectionner des éléments
                listBox.SelectedItem(2, true);  // Select third item (index 2)
                listBox.SelectedItem(0, true);   // Select first item (index 0)
                listBox.SelectedItem(2, false); // Deselect third item

                // Vérifier les sélections
                Console.WriteLine($"Item 0 selected: {listBox.IsSelected(0)}");
                Console.WriteLine($"Item 2 selected: {listBox.IsSelected(2)}");

                // Afficher les cellules sélectionnées
                Console.WriteLine("\nSelected Items:");
                foreach (Cell cell in listBox.SelectedCells)
                {
                    Console.WriteLine(cell.Value);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ListBoxMethodSelectedItemWithInt32BooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



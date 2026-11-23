---
title: "ComboBox.SelectedIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ComboBox. Obtient ou définit le numéro d'index de l'élément actuellement sélectionné dans une zone de liste ou une boîte combinée. Index zéro basé"
type: docs
url: /fr/net/aspose.cells.drawing/combobox/selectedindex/
---
## ComboBox.SelectedIndex property

Obtient ou définit le numéro d'index de l'élément actuellement sélectionné dans une zone de liste ou une zone combinée. Indexé à partir de zéro.

```csharp
public int SelectedIndex { get; set; }
```

### Remarques

-1 presents no item is selected.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertySelectedIndexDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour la boîte combinée
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");

            // Ajouter une boîte combinée à la feuille de calcul
            Shape shape = worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 20);
            ComboBox comboBox = (ComboBox)shape;

            // Définir la plage d'entrée pour la boîte combinée
            comboBox.InputRange = "A1:A5";
            comboBox.DropDownLines = 5;

            // Définir et afficher l'index sélectionné
            comboBox.SelectedIndex = 2; // Selects "Item 3" (zero-based index)
            Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
            Console.WriteLine("Selected Value: " + comboBox.SelectedValue);

            // Modifier l'index sélectionné et l'afficher à nouveau
            comboBox.SelectedIndex = 4; // Selects "Item 5"
            Console.WriteLine("\nAfter changing selection:");
            Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
            Console.WriteLine("Selected Value: " + comboBox.SelectedValue);
        }
    }
}
```

### Voir aussi

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



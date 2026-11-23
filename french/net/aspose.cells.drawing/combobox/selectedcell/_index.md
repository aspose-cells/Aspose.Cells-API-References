---
title: "ComboBox.SelectedCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ComboBox. Obtient la cellule sélectionnée dans la plage d'entrée du combobox"
type: docs
url: /fr/net/aspose.cells.drawing/combobox/selectedcell/
---
## ComboBox.SelectedCell property

Obtient la cellule sélectionnée dans la plage d'entrée de la boîte combinée.

```csharp
public Cell SelectedCell { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ComboBoxPropertySelectedCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir les cellules avec des données d'exemple pour les éléments du combobox
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["A4"].PutValue("Date");
            worksheet.Cells["A5"].PutValue("Fig");

            // Créer un ComboBox et définir ses propriétés
            ComboBox comboBox = worksheet.Shapes.AddComboBox(0, 0, 100, 100, 5, 0);
            comboBox.InputRange = "A1:A5";
            comboBox.DropDownLines = 5;

            // Définir la sélection et démontrer SelectedCell
            comboBox.SelectedIndex = 2;
            Cell selectedCell = comboBox.SelectedCell;

            Console.WriteLine($"Initial Selected Cell Value: {selectedCell.StringValue}");

            // Modifier la valeur de la cellule sélectionnée
            selectedCell.PutValue("Orange");
            Console.WriteLine($"Updated Selected Cell Value: {selectedCell.StringValue}");

            // Afficher l'effet sur les cellules adjacentes
            worksheet.Cells["B3"].PutValue($"Combo Selection: {comboBox.SelectedValue}");

            workbook.Save("ComboBoxSelectedCellDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../../../aspose.cells/cell/)
* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



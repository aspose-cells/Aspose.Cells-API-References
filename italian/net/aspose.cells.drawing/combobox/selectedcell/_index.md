---
title: "ComboBox.SelectedCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ComboBox. Restituisce la cella selezionata nell'intervallo di input del combo box"
type: docs
url: /it/net/aspose.cells.drawing/combobox/selectedcell/
---
## ComboBox.SelectedCell property

Ottiene la cella selezionata nell'intervallo di input della casella combinata.

```csharp
public Cell SelectedCell { get; }
```

### Esempi

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

            // Popola le celle con dati di esempio per gli elementi del combobox
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["A4"].PutValue("Date");
            worksheet.Cells["A5"].PutValue("Fig");

            // Crea un ComboBox e imposta le sue proprietà
            ComboBox comboBox = worksheet.Shapes.AddComboBox(0, 0, 100, 100, 5, 0);
            comboBox.InputRange = "A1:A5";
            comboBox.DropDownLines = 5;

            // Imposta la selezione e dimostra SelectedCell
            comboBox.SelectedIndex = 2;
            Cell selectedCell = comboBox.SelectedCell;

            Console.WriteLine($"Initial Selected Cell Value: {selectedCell.StringValue}");

            // Modifica il valore della cella selezionata
            selectedCell.PutValue("Orange");
            Console.WriteLine($"Updated Selected Cell Value: {selectedCell.StringValue}");

            // Mostra l'effetto sulle celle adiacenti
            worksheet.Cells["B3"].PutValue($"Combo Selection: {comboBox.SelectedValue}");

            workbook.Save("ComboBoxSelectedCellDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../../../aspose.cells/cell/)
* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



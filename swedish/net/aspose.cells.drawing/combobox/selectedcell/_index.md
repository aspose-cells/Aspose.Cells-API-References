---
title: "ComboBox.SelectedCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBox-egenskap. Hämtar den markerade cellen i inmatningsintervallet för comboboxen"
type: docs
url: /sv/net/aspose.cells.drawing/combobox/selectedcell/
---
## ComboBox.SelectedCell property

Hämtar den valda cellen i inmatningsintervallet för kombinationsrutan.

```csharp
public Cell SelectedCell { get; }
```

### Exempel

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

            // Fyll celler med exempeldata för combobox-objekt
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["A4"].PutValue("Date");
            worksheet.Cells["A5"].PutValue("Fig");

            // Skapa en ComboBox och ange dess egenskaper
            ComboBox comboBox = worksheet.Shapes.AddComboBox(0, 0, 100, 100, 5, 0);
            comboBox.InputRange = "A1:A5";
            comboBox.DropDownLines = 5;

            // Ange markering och demonstrera SelectedCell
            comboBox.SelectedIndex = 2;
            Cell selectedCell = comboBox.SelectedCell;

            Console.WriteLine($"Initial Selected Cell Value: {selectedCell.StringValue}");

            // Ändra det markerade cellens värde
            selectedCell.PutValue("Orange");
            Console.WriteLine($"Updated Selected Cell Value: {selectedCell.StringValue}");

            // Visa effekten på intilliggande celler
            worksheet.Cells["B3"].PutValue($"Combo Selection: {comboBox.SelectedValue}");

            workbook.Save("ComboBoxSelectedCellDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../../../aspose.cells/cell/)
* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



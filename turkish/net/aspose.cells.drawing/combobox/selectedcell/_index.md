---
title: "ComboBox.SelectedCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ComboBox özelliği. ComboBox'ın giriş aralığındaki seçili hücreyi alır"
type: docs
url: /tr/net/aspose.cells.drawing/combobox/selectedcell/
---
## ComboBox.SelectedCell property

Combo kutusunun giriş aralığındaki seçili hücreyi alır.

```csharp
public Cell SelectedCell { get; }
```

### Örnekler

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

            // ComboBox öğeleri için örnek veri ile hücreleri doldurun
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["A4"].PutValue("Date");
            worksheet.Cells["A5"].PutValue("Fig");

            // Bir ComboBox oluşturun ve özelliklerini ayarlayın
            ComboBox comboBox = worksheet.Shapes.AddComboBox(0, 0, 100, 100, 5, 0);
            comboBox.InputRange = "A1:A5";
            comboBox.DropDownLines = 5;

            // Seçimi ayarlayın ve SelectedCell'ı gösterin
            comboBox.SelectedIndex = 2;
            Cell selectedCell = comboBox.SelectedCell;

            Console.WriteLine($"Initial Selected Cell Value: {selectedCell.StringValue}");

            // Seçili hücrenin değerini değiştirin
            selectedCell.PutValue("Orange");
            Console.WriteLine($"Updated Selected Cell Value: {selectedCell.StringValue}");

            // Komşu hücrelerdeki etkiyi gösterin
            worksheet.Cells["B3"].PutValue($"Combo Selection: {comboBox.SelectedValue}");

            workbook.Save("ComboBoxSelectedCellDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../../aspose.cells/cell/)
* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



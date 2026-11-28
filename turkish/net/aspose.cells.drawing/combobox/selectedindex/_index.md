---
title: "ComboBox.SelectedIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ComboBox özelliği. Bir liste kutusunda veya combo kutusunda şu anda seçili öğenin indeks numarasını alır veya ayarlar. Sıfır tabanlı"
type: docs
url: /tr/net/aspose.cells.drawing/combobox/selectedindex/
---
## ComboBox.SelectedIndex property

Liste kutusunda veya combo kutusunda şu anda seçili öğenin dizin numarasını alır veya ayarlar. Sıfır tabanlı.

```csharp
public int SelectedIndex { get; set; }
```

### Açıklamalar

-1 presents no item is selected.

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Combo kutusu için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");

            // Çalışma sayfasına bir combo kutusu ekleyin
            Shape shape = worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 20);
            ComboBox comboBox = (ComboBox)shape;

            // Combo kutusu için giriş aralığını ayarlayın
            comboBox.InputRange = "A1:A5";
            comboBox.DropDownLines = 5;

            // Seçili indeksi ayarlayın ve görüntüleyin
            comboBox.SelectedIndex = 2; // Selects "Item 3" (zero-based index)
            Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
            Console.WriteLine("Selected Value: " + comboBox.SelectedValue);

            // Seçili indeksi değiştirin ve tekrar görüntüleyin
            comboBox.SelectedIndex = 4; // Selects "Item 5"
            Console.WriteLine("\nAfter changing selection:");
            Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
            Console.WriteLine("Selected Value: " + comboBox.SelectedValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



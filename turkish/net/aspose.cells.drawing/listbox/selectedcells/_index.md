---
title: "ListBox.SelectedCells"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListBox özelliği. Seçili hücreleri alır. Giriş aralığı ayarlanmamışsa veya hiçbir öğe seçilmemişse null döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/listbox/selectedcells/
---
## ListBox.SelectedCells property

Seçili hücreleri alır. Giriş aralığı ayarlanmamışsa veya hiçbir öğe seçilmemişse null döndürür.

```csharp
public Cell[] SelectedCells { get; }
```

### Örnekler

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

            // ListBox öğeleri için örnek veri doldur
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");

            // Bir ListBox oluştur ve veri aralığına bağla
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(7, 0, 100, 150, 5, 1);
            listBox.InputRange = "A1:A5";
            listBox.SelectionType = SelectionType.Multi;

            // Sıfır tabanlı indeksler kullanarak birden fazla öğe seç
            listBox.SelectedItem(0, true);
            listBox.SelectedItem(2, true);

            // Seçili hücreleri al ve göster
            Cell[] selectedCells = listBox.SelectedCells;
            Console.WriteLine("Selected Cells Count: " + selectedCells.Length);
            
            // Erişimi göstermek için seçili hücreleri değiştir
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

### Ayrıca Bakınız

* class [Cell](../../../aspose.cells/cell/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



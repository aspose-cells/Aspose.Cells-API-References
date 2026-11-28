---
title: "ListBox.SelectedItem"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListBox yöntemi. Öğenin seçili olup olmadığını ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/listbox/selecteditem/
---
## ListBox.SelectedItem method

Öğenin seçili olup olmadığını ayarlar

```csharp
public void SelectedItem(int itemIndex, bool isSelected)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| itemIndex | Int32 | Öğe indeksi |
| isSelected | Boolean | Öğenin seçili olup olmadığını belirtir. True, bu öğenin seçilmesi gerektiği anlamına gelir. False, bu öğenin seçilmemesi gerektiği anlamına gelir. |

### Örnekler

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

            // Liste öğelerini doldur
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i, 0].Value = $"Item {i + 1}";
            }

            // Liste kutusu oluştur
            ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 150, 100) as ListBox;
            listBox.InputRange = "A1:A5";
            listBox.SelectionType = SelectionType.Multi;

            try
            {
                // Öğeleri seç ve seçimini kaldır
                listBox.SelectedItem(2, true);  // Select third item (index 2)
                listBox.SelectedItem(0, true);   // Select first item (index 0)
                listBox.SelectedItem(2, false); // Deselect third item

                // Seçimleri doğrula
                Console.WriteLine($"Item 0 selected: {listBox.IsSelected(0)}");
                Console.WriteLine($"Item 2 selected: {listBox.IsSelected(2)}");

                // Seçili hücreleri göster
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

### Ayrıca Bakınız

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



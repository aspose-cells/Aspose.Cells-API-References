---
title: "ListBox.IsSelected"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListBox yöntemi. Öğenin seçili olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/listbox/isselected/
---
## ListBox.IsSelected method

Öğenin seçili olup olmadığını gösterir.

```csharp
public bool IsSelected(int itemIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| itemIndex | Int32 | Öğe indeksi. |

### Dönüş Değeri

öğenin seçili olup olmadığı.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxMethodIsSelectedWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir liste kutusu ekle
            ListBox listBox = worksheet.Shapes.AddListBox(0, 0, 100, 100, 200, 200);

            // Bağlı hücre aralığı üzerinden liste öğelerini ayarla
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            listBox.LinkedCell = "A1:A3";

            // Bir öğe seçin
            listBox.SelectedIndex = 0;

            // Int32 parametresiyle IsSelected kullanarak seçim durumunu kontrol edin
            Console.WriteLine("Item 0 selected: " + listBox.IsSelected(0));
            Console.WriteLine("Item 1 selected: " + listBox.IsSelected(1));
            Console.WriteLine("Item 2 selected: " + listBox.IsSelected(2));
        }
    }
}
```

### Ayrıca Bakınız

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)



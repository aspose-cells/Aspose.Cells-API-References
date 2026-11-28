---
title: "Enum SelectionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.SelectionType enum. List kutusunun seçim türü"
type: docs
url: /tr/net/aspose.cells.drawing/selectiontype/
---
## SelectionType enumeration

Liste kutusunun seçim tipini.

```csharp
public enum SelectionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Single | `0` | Tek seçim türü. |
| Multi | `1` | Çoklu seçim türü. |
| Extend | `2` | Seçim türünü genişlet. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassSelectionTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir liste kutusu ekle
            ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 5, 10);

            // Seçim türünü Tek olarak ayarla
            listBox.SelectionType = SelectionType.Single;

            // Liste kutusuna öğeler ekle
            listBox.SetInputRange("A1:A5", false, false);

            // Seçim türünü doğrula
            Console.WriteLine("ListBox SelectionType: " + listBox.SelectionType);

            // Çalışma kitabını kaydedin
            workbook.Save("SelectionTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



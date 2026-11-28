---
title: "DataSorterKey.Color"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorterKey özelliği. Sıralanmış rengi alır"
type: docs
url: /tr/net/aspose.cells/datasorterkey/color/
---
## DataSorterKey.Color property

Sıralanmış rengi alır.

```csharp
public Color Color { get; }
```

### Açıklamalar

Yalnızca [`Type`](../type/) CellColor veya FontColor olduğunda etkili olur.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyColorDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı nesnesi oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Veri sıralayıcı oluştur ve anahtar ekle
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Verileri sırala
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Anahtarlardan renk özelliğini çıktı olarak al
            foreach (DataSorterKey k in sorter.Keys)
            {
                Console.WriteLine($"Color: {k.Color}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



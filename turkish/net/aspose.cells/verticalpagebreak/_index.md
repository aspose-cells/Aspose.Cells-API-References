---
title: "Sınıf VerticalPageBreak"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.VerticalPageBreak sınıfı. Dikey sayfa sonunu temsil eden nesneyi kapsar."
type: docs
url: /tr/net/aspose.cells/verticalpagebreak/
---
## VerticalPageBreak class

Dikey sayfa sonunu temsil eden nesneyi kapsüller.

```csharp
public class VerticalPageBreak
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Column](../../aspose.cells/verticalpagebreak/column/) { get; } | Dikey sayfa sonunun sütun indeksini alır. |
| [EndRow](../../aspose.cells/verticalpagebreak/endrow/) { get; } | Dikey sayfa sonunun bitiş satır indeksini alır. |
| [StartRow](../../aspose.cells/verticalpagebreak/startrow/) { get; } | Dikey sayfa sonunun başlangıç satır indeksini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakDemo
    {
        public static void VerticalPageBreakExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabındaki ilk çalışma sayfasına erişin
            Worksheet worksheet = workbook.Worksheets[0];
            
            // G sütununda (indeks 6) bir dikey sayfa sonu ekle
            worksheet.VerticalPageBreaks.Add("G5");

            // Çalışma kitabını kaydedin
            workbook.Save("VerticalPageBreakExample.xlsx");

            // Eklenen dikey sayfa sonuna eriş
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];

            // Dikey sayfa sonunun özelliklerini göster
            Console.WriteLine("Start Row: " + vpb.StartRow);
            Console.WriteLine("End Row: " + vpb.EndRow);
            Console.WriteLine("Column: " + vpb.Column);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



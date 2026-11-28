---
title: "Sınıf CellWatch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CellWatch sınıfı. İzleme penceresinde Hücre İzleme Öğesini temsil eder"
type: docs
url: /tr/net/aspose.cells/cellwatch/
---
## CellWatch class

'watch window' içinde Hücre İzleme Öğesini temsil eder.

```csharp
public class CellWatch
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [CellWatch](cellwatch/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CellName](../../aspose.cells/cellwatch/cellname/) { get; set; } | Hücrenin adını alır ve ayarlar. |
| [Column](../../aspose.cells/cellwatch/column/) { get; set; } | Hücrenin sütununu alır ve ayarlar. |
| [Row](../../aspose.cells/cellwatch/row/) { get; set; } | Hücrenin satırını alır ve ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchDemo
    {
        public static void CellWatchExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            // İlk Çalışma Sayfasını al.
            Worksheet sheet = workbook.Worksheets[0];

            // Hücre İzleme Öğesini izleme penceresine ekle
            int watchIndex = sheet.CellWatches.Add("B2");

            // CellWatch nesnesini al
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Özellikleri ayarlama
            cellWatch.Row = 1; // B2 corresponds to row 1 (0-based index)
            cellWatch.Column = 1; // B2 corresponds to column 1 (0-based index)
            cellWatch.CellName = "B2";

            // Çalışma kitabını kaydedin
            workbook.Save("CellWatchExample.xlsx");
            workbook.Save("CellWatchExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



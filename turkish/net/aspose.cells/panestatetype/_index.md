---
title: "Enum PaneStateType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.PaneStateType enum. Sayfa bölmesinin durumunu temsil eder"
type: docs
url: /tr/net/aspose.cells/panestatetype/
---
## PaneStateType enumeration

Sayfanın bölmesinin durumunu temsil eder.

```csharp
public enum PaneStateType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Frozen | `0` | Bölmeler dondurulmuş, ancak dondurulmadan önce dondurulmamıştı. |
| FrozenSplit | `1` | Bölmeler dondurulmuş ve dondurulmadan önce bölünmüştü. |
| Split | `2` | Bölmeler bölünmüş, ancak dondurulmamış. |
| Normal | `3` | Bölmeler dondurulmamış ve bölünmemiş. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PaneStateTypeDemo
    {
        public static void PaneStateTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı örnek veriler ayarla
            worksheet.Cells["A1"].PutValue("Data 1");
            worksheet.Cells["A2"].PutValue("Data 2");
            worksheet.Cells["A3"].PutValue("Data 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // B2 hücresinde bölmeleri dondur
            worksheet.FreezePanes(1, 0, 1, 1); // Freeze the first row and first column

            // Bölme durumunu kontrol et
            PaneStateType paneState = worksheet.PaneState;

            // Bölme durumunu çıktı olarak ver
            Console.WriteLine("Current Pane State: " + paneState);

            // Çalışma kitabını kaydedin
            workbook.Save("PaneStateTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



---
title: "Enum DateTimeGroupingType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DateTimeGroupingType enum. DateTime değerlerinin nasıl gruplanacağını belirtir"
type: docs
url: /tr/net/aspose.cells/datetimegroupingtype/
---
## DateTimeGroupingType enumeration

dateTime değerlerinin nasıl gruplanacağını belirtir.

```csharp
public enum DateTimeGroupingType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Day | `0` | Gün bazında grupla. |
| Hour | `1` | Saat bazında grupla. |
| Minute | `2` | Dakika bazında grupla. |
| Month | `3` | Ay bazında grupla. |
| Second | `4` | Saniye bazında grupla. |
| Year | `5` | Yıl bazında grupla |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupingTypeDemo
    {
        public static void DateTimeGroupingTypeExample()
        {
            // Bir çalışma kitabı oluşturma ve ilk çalışma sayfasına erişme
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bazı örnek veriler ekleme
            worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1, 10, 0, 0));
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1, 11, 0, 0));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2, 10, 0, 0));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 1, 2, 11, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 2, 1, 10, 0, 0));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 2, 1, 11, 0, 0));

            // Bir AutoFilter oluşturma ve aralığı ayarlama
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:A6";

            // Farklı DateTimeGroupingType ile tarih filtreleri ekleme
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Month, 2023, 1, 1, 0, 0, 0);
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Hour, 2023, 1, 1, 10, 0, 0);
            
            // Çalışma kitabını kaydetme
            workbook.Save("DateTimeGroupingTypeExample.xlsx");
            workbook.Save("DateTimeGroupingTypeExample.pdf");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



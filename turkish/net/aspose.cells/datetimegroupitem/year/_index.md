---
title: "DateTimeGroupItem.Year"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DateTimeGroupItem özelliği. Gruplanmış tarih saatinin yılını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/datetimegroupitem/year/
---
## DateTimeGroupItem.Year property

Gruplanmış tarih saatinin yılını alır ve ayarlar.

```csharp
public int Year { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyYearDemo
    {
        public static void Run()
        {
            // Yıla göre gruplanmış bir DateTimeGroupItem oluştur
            DateTimeGroupItem dateTimeGroup = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,  // Year
                1,     // Month (ignored when grouping by Year)
                1,     // Day (ignored)
                0,     // Hour (ignored)
                0,     // Minute (ignored)
                0      // Second (ignored)
            );

            // İlk Yıl değerini göster
            Console.WriteLine("Initial Year: " + dateTimeGroup.Year);

            // Yıl özelliğini değiştir
            dateTimeGroup.Year = 2024;

            // Değiştirilmiş Yıl değerini göster
            Console.WriteLine("Modified Year: " + dateTimeGroup.Year);

            // Yıla göre gruplandırıldığında diğer özelliklerin yoksayıldığını göster
            dateTimeGroup.Month = 12;
            Console.WriteLine("Month value is ignored when grouping by Year: " + dateTimeGroup.Month);
        }
    }
}
```

### Ayrıca Bakınız

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



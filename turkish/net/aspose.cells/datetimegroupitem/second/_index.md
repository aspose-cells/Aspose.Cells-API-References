---
title: "DateTimeGroupItem.Second"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DateTimeGroupItem özelliği. Gruplanmış tarih saatinin saniyesini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/datetimegroupitem/second/
---
## DateTimeGroupItem.Second property

Gruplanmış tarih saatinin saniyesini alır ve ayarlar.

```csharp
public int Second { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertySecondDemo
    {
        public static void Run()
        {
            // DateTimeGroupItem örneği oluştur
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year, // Group by Year
                2023,                      // Year
                10,                        // Month
                5,                         // Day
                14,                        // Hour
                30,                        // Minute
                45                         // Second
            );

            // İlk saniye değerini göster
            Console.WriteLine("Initial Second: " + dateTimeGroupItem.Second);

            // Saniye değerini değiştir
            dateTimeGroupItem.Second = 50;
            Console.WriteLine("Modified Second: " + dateTimeGroupItem.Second);

            // Farklı saniye değeriyle başka bir örnek oluştur
            DateTimeGroupItem anotherItem = new DateTimeGroupItem(
                DateTimeGroupingType.Day,
                2023,
                10,
                5,
                14,
                30,
                0  // Second set to 0
            );
            Console.WriteLine("Another Item Second: " + anotherItem.Second);
        }
    }
}
```

### Ayrıca Bakınız

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



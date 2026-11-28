---
title: "DateTimeGroupItem.Day"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DateTimeGroupItem özelliği. Gruplanmış tarih zamanının gününü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/datetimegroupitem/day/
---
## DateTimeGroupItem.Day property

Gruplanmış tarih saatinin gününü alır ve ayarlar.

```csharp
public int Day { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyDayDemo
    {
        public static void Run()
        {
            // Yıla göre gruplanmış bir DateTimeGroupItem oluştur
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,  // Year
                10,    // Month
                5,     // Day
                14,    // Hour
                30,    // Minute
                45     // Second
            );

            // İlk gün değerini göster
            Console.WriteLine("Initial Day: " + dateTimeGroupItem.Day);

            // Gün özelliğini değiştir
            dateTimeGroupItem.Day = 25;
            Console.WriteLine("Modified Day: " + dateTimeGroupItem.Day);

            // Gün özelliğinin önemini göstermek için Gün'e göre gruplanmış başka bir DateTimeGroupItem oluştur
            DateTimeGroupItem dayGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Day,
                2023,
                10,
                15,  // Initial day
                0,
                0,
                0
            );

            Console.WriteLine("\nDay-grouped item initial Day: " + dayGroupItem.Day);
            dayGroupItem.Day = 20;
            Console.WriteLine("Day-grouped item modified Day: " + dayGroupItem.Day);
        }
    }
}
```

### Ayrıca Bakınız

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



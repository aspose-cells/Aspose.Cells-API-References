---
title: "DateTimeGroupItem.Hour"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DateTimeGroupItem özelliği. Gruplanmış tarih saatinin saatini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/datetimegroupitem/hour/
---
## DateTimeGroupItem.Hour property

Gruplanmış tarih saatinin saatini alır ve ayarlar.

```csharp
public int Hour { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyHourDemo
    {
        public static void Run()
        {
            // Saat gruplamasıyla bir DateTimeGroupItem oluştur
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Hour,
                2023,  // Year
                10,     // Month
                5,      // Day
                14,     // Hour
                0,      // Minute
                0      // Second
            );

            // İlk saat değerini göster
            Console.WriteLine("Initial Hour: " + dateTimeGroupItem.Hour);

            // Saat özelliğini değiştir
            dateTimeGroupItem.Hour = 18;

            // Değiştirilmiş saat değerini göster
            Console.WriteLine("Modified Hour: " + dateTimeGroupItem.Hour);
        }
    }
}
```

### Ayrıca Bakınız

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



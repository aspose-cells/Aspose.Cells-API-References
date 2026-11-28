---
title: "DateTimeGroupItem.Minute"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DateTimeGroupItem özelliği. Gruplanmış tarih zamanının dakikasını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/datetimegroupitem/minute/
---
## DateTimeGroupItem.Minute property

Gruplanmış tarih saatinin dakikasını alır ve ayarlar.

```csharp
public int Minute { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMinuteDemo
    {
        public static void Run()
        {
            // İlk değerlerle bir DateTimeGroupItem oluştur
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,
                10,
                5,
                14,
                30,
                45
            );

            // İlk dakika değerini göster
            Console.WriteLine("Initial Minute: " + dateTimeGroupItem.Minute);

            // Dakika değerini değiştir
            dateTimeGroupItem.Minute = 15;

            // Değiştirilmiş dakika değerini göster
            Console.WriteLine("Modified Minute: " + dateTimeGroupItem.Minute);

            // Sadece dakika gruplanmasıyla yeni bir DateTimeGroupItem oluştur
            DateTimeGroupItem minuteGroup = new DateTimeGroupItem(
                DateTimeGroupingType.Minute,
                0, 0, 0, 0, 45, 0
            );

            // Dakika grubundan dakikayı göster
            Console.WriteLine("Minute from Minute Grouping: " + minuteGroup.Minute);
        }
    }
}
```

### Ayrıca Bakınız

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



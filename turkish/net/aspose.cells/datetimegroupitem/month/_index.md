---
title: "DateTimeGroupItem.Month"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DateTimeGroupItem özelliği. Gruplanmış tarih zamanının ayını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/datetimegroupitem/month/
---
## DateTimeGroupItem.Month property

Gruplanmış tarih saatinin ayını alır ve ayarlar.

```csharp
public int Month { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMonthDemo
    {
        public static void Run()
        {
            // Ay'a göre gruplanmış bir DateTimeGroupItem oluştur
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Month,
                2023,
                10,
                1,
                0,
                0,
                0
            );

            // İlk ay değerini göster
            Console.WriteLine("Initial Month: " + dateTimeGroupItem.Month);

            // Ay değerini değiştir
            dateTimeGroupItem.Month = 12;
            Console.WriteLine("Modified Month: " + dateTimeGroupItem.Month);

            // Farklı gruplayarak başka bir DateTimeGroupItem oluştur
            DateTimeGroupItem yearlyItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,
                1,
                1,
                0,
                0,
                0
            );

            // Ay özelliğinin, Yıla göre gruplanmış olsa bile hâlâ erişilebilir olduğunu göster
            Console.WriteLine("Yearly Grouping - Month: " + yearlyItem.Month);
        }
    }
}
```

### Ayrıca Bakınız

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



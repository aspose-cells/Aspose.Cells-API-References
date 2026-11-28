---
title: "Sınıf DateTimeGroupItem"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DateTimeGroupItem sınıfı. Tarih saat grup ayarını temsil eder"
type: docs
url: /tr/net/aspose.cells/datetimegroupitem/
---
## DateTimeGroupItem class

Tarih saat grubu ayarını temsil eder.

```csharp
public class DateTimeGroupItem
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [DateTimeGroupItem](datetimegroupitem/)(DateTimeGroupingType, int, int, int, int, int, int) |  |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DateTimeGroupingType](../../aspose.cells/datetimegroupitem/datetimegroupingtype/) { get; set; } | Grup tipini alır ve ayarlar. |
| [Day](../../aspose.cells/datetimegroupitem/day/) { get; set; } | Gruplanmış tarih saatinin gününü alır ve ayarlar. |
| [Hour](../../aspose.cells/datetimegroupitem/hour/) { get; set; } | Gruplanmış tarih saatinin saatini alır ve ayarlar. |
| [Minute](../../aspose.cells/datetimegroupitem/minute/) { get; set; } | Gruplanmış tarih saatinin dakikasını alır ve ayarlar. |
| [MinValue](../../aspose.cells/datetimegroupitem/minvalue/) { get; } | Minimum değeri alır. |
| [Month](../../aspose.cells/datetimegroupitem/month/) { get; set; } | Gruplanmış tarih saatinin ayını alır ve ayarlar. |
| [Second](../../aspose.cells/datetimegroupitem/second/) { get; set; } | Gruplanmış tarih saatinin saniyesini alır ve ayarlar. |
| [Year](../../aspose.cells/datetimegroupitem/year/) { get; set; } | Gruplanmış tarih saatinin yılını alır ve ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupItemDemo
    {
        public static void DateTimeGroupItemExample()
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

            // Özelliklere erişim
            Console.WriteLine("MinValue: " + dateTimeGroupItem.MinValue);
            Console.WriteLine("DateTimeGroupingType: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Year: " + dateTimeGroupItem.Year);
            Console.WriteLine("Month: " + dateTimeGroupItem.Month);
            Console.WriteLine("Day: " + dateTimeGroupItem.Day);
            Console.WriteLine("Hour: " + dateTimeGroupItem.Hour);
            Console.WriteLine("Minute: " + dateTimeGroupItem.Minute);
            Console.WriteLine("Second: " + dateTimeGroupItem.Second);

            // Özellikleri değiştirme
            dateTimeGroupItem.DateTimeGroupingType = DateTimeGroupingType.Month;
            dateTimeGroupItem.Year = 2022;
            dateTimeGroupItem.Month = 12;
            dateTimeGroupItem.Day = 25;
            dateTimeGroupItem.Hour = 10;
            dateTimeGroupItem.Minute = 15;
            dateTimeGroupItem.Second = 30;

            // Değiştirilmiş özelliklere erişim
            Console.WriteLine("Modified DateTimeGroupingType: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Modified Year: " + dateTimeGroupItem.Year);
            Console.WriteLine("Modified Month: " + dateTimeGroupItem.Month);
            Console.WriteLine("Modified Day: " + dateTimeGroupItem.Day);
            Console.WriteLine("Modified Hour: " + dateTimeGroupItem.Hour);
            Console.WriteLine("Modified Minute: " + dateTimeGroupItem.Minute);
            Console.WriteLine("Modified Second: " + dateTimeGroupItem.Second);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



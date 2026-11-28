---
title: "DateTimeGroupItem.DateTimeGroupItem"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DateTimeGroupItem yapıcı."
type: docs
url: /tr/net/aspose.cells/datetimegroupitem/datetimegroupitem/
---
## DateTimeGroupItem constructor

```csharp
public DateTimeGroupItem(DateTimeGroupingType type, int year, int month, int day, int hour, 
    int minute, int second)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | DateTimeGroupingType |  |
| yıl | Int32 |  |
| ay | Int32 |  |
| gün | Int32 |  |
| saat | Int32 |  |
| dakika | Int32 |  |
| saniye | Int32 |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupItemMethodCtorWithDateTimeGroupingTypeInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A sütununa örnek tarih saat verileri ekle
            worksheet.Cells["A1"].PutValue("Order Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 3, 15, 9, 30, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 4, 20, 14, 15, 45));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 25, 10, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2024, 3, 1, 8, 45, 30));

            // Tarih sütununa otomatik filtre uygula
            worksheet.AutoFilter.Range = "A1:A5";

            try
            {
                // Mart 2023 gruplandırması için DateTimeGroupItem oluştur
                DateTimeGroupItem groupItem = new DateTimeGroupItem(
                    DateTimeGroupingType.Month, // Group by Month
                    2023,   // Year
                    3,      // Month (March)
                    1,      // Day (ignored in Month grouping)
                    0,      // Hour
                    0,      // Minute
                    0       // Second
                );

                // Filtreyi Mart 2023 tarihlerini gösterecek şekilde yapılandır
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
                filterColumn.FilterType = FilterType.MultipleFilters;
                filterColumn.Filter = groupItem;

                // Değişiklikleri uygulamak için filtreyi yenile
                worksheet.AutoFilter.Refresh();

                Console.WriteLine("DateTimeGroupItem created and filter applied successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error applying date filter: {ex.Message}");
            }

            // Filtrelenmiş çalışma kitabını kaydet
            workbook.Save("DateTimeGroupItemConstructorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



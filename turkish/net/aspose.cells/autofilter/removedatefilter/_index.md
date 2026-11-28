---
title: "AutoFilter.RemoveDateFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFilter yöntemi. Bir tarih filtresini kaldırır"
type: docs
url: /tr/net/aspose.cells/autofilter/removedatefilter/
---
## AutoFilter.RemoveDateFilter method

Bir tarih filtresini kaldırır.

```csharp
public void RemoveDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
    int month, int day, int hour, int minute, int second)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldIndex | Int32 | Filtreyi temellendirmek istediğiniz alanın tam sayı ofseti (listenin solundan; en soldaki alan field 0'dır). |
| dateTimeGroupingType | DateTimeGroupingType | Gruplama türü |
| yıl | Int32 | Yıl. |
| ay | Int32 | Ay. |
| gün | Int32 | Gün. |
| saat | Int32 | Saat. |
| dakika | Int32 | Dakika. |
| saniye | Int32 | Saniye. |

### Açıklamalar

DateTimeGroupingType Yıl ise, yalnızca yıl parametresi etkili olur. DateTiemGroupingType Ay ise, yalnızca yıl ve ay parametreleri etkili olur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRemoveDateFilterWithInt32DateTimeGroupingTypeInt32Demo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Tarihlerle örnek veri ekle
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue(new DateTime(2020, 1, 7));
            sheet.Cells["A3"].PutValue(new DateTime(2020, 1, 8));
            sheet.Cells["A4"].PutValue(new DateTime(2020, 1, 9));
            
            // Otomatik filtre uygula
            sheet.AutoFilter.Range = "A1:A4";
            
            // 7. gün için tarih filtresi ekle
            sheet.AutoFilter.AddDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            sheet.AutoFilter.Refresh();
            
            // Filtrenin uygulandığını doğrula
            Console.WriteLine("Row 2 hidden: " + sheet.Cells.IsRowHidden(1)); // Should be true
            
            // Tarih filtresini kaldır
            sheet.AutoFilter.RemoveDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            sheet.AutoFilter.Refresh();
            
            // Filtrenin kaldırıldığını doğrula
            Console.WriteLine("Row 2 hidden after removal: " + sheet.Cells.IsRowHidden(1)); // Should be false
        }
    }
}
```

### Ayrıca Bakınız

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)



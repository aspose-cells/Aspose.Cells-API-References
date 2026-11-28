---
title: "Enum PivotGroupByType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotGroupByType enum. Grup oluşturma tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivotgroupbytype/
---
## PivotGroupByType enumeration

Gruplama türünü temsil eder.

```csharp
[Flags]
public enum PivotGroupByType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| RangeOfValues | `1` | Sayılara göre gruplandır. |
| Numbers | `1` | Sayılara göre gruplandır. |
| Seconds | `2` | Saniyeler grup tipini sunar. |
| Minutes | `4` | Dakikalar grup tipini sunar. |
| Hours | `8` | Saatler grup tipini sunar. |
| Days | `10` | Günler grup tipini sunar. |
| Months | `20` | Aylar grup tipini sunar. |
| Quarters | `40` | Çeyrekler grup tipini sunar. |
| Years | `80` | Yıllar grup tipini sunar. |
| DateTimes | `FE` | Tarih zamanların tüm grup tiplerini sunar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotGroupByTypeDemo
    {
        public static void PivotGroupByTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Date");
            Style style = workbook.CreateStyle();
            style.Number = 14;//m/d/yyy
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A2"].SetStyle(style);

            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A3"].SetStyle(style);

            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A4"].SetStyle(style);

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir pivot tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Pivot tabloya alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value field

            //YAPILACAK
            PivotField dateField = pivotTable.RowFields[0];

            DateTime start = new DateTime(2023, 1, 1);
            DateTime end = new DateTime(2023, 12, 31);
            dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, false);

            // Grup ayarlarına eriş
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

            // Grup ayarlarını çıktıla
            Console.WriteLine("Group Type: " + groupSettings.Type);
            Console.WriteLine("Start Date: " + groupSettings.Start);
            Console.WriteLine("End Date: " + groupSettings.End);
            Console.WriteLine("Interval: " + groupSettings.Interval);
            Console.WriteLine("Is Grouped By Months: " + groupSettings.IsGroupedBy(PivotGroupByType.Months));

            // Çalışma kitabını kaydedin
            workbook.Save("PivotGroupByTypeExample.xlsx");
            
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)



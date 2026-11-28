---
title: "Enum TimePeriodType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.TimePeriodType enum. FormatConditionType.TimePeriod koşullu biçimlendirme kuralında kullanılır. Bunlar, koşullu biçimlendirmenin yenilendiği / uygulandığı tarihe göre değişen dinamik zaman periyotlarıdır."
type: docs
url: /tr/net/aspose.cells/timeperiodtype/
---
## TimePeriodType enumeration

FormatConditionType.TimePeriod koşullu biçimlendirme kuralında kullanılır. Bunlar, koşullu biçimlendirme yenilendiğinde/uygulandığında tarihe göre değişen dinamik zaman dilimleridir.

```csharp
public enum TimePeriodType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Today | `0` | Bugünün tarihi. |
| Yesterday | `1` | Dünün tarihi. |
| Tomorrow | `2` | Yarının tarihi. |
| Last7Days | `3` | Son yedi gün içindeki bir tarih. |
| ThisMonth | `4` | Bu takvim ayında gerçekleşen bir tarih. |
| LastMonth | `5` | Geçen takvim ayında gerçekleşen bir tarih. |
| NextMonth | `6` | Gelecek takvim ayında gerçekleşen bir tarih. |
| ThisWeek | `7` | Bu hafta gerçekleşen bir tarih. |
| LastWeek | `8` | Geçen hafta gerçekleşen bir tarih. |
| NextWeek | `9` | Gelecek hafta gerçekleşen bir tarih. |
| ThisYear | `10` | Bu yıl gerçekleşen bir tarih. Yalnızca .ods için. |
| LastYear | `11` | Geçen yıl gerçekleşen bir tarih. Yalnızca .ods için. |
| NextYear | `12` | Gelecek yıl gerçekleşen bir tarih. Yalnızca .ods için. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TimePeriodTypeDemo
    {
        public static void TimePeriodTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Koşullu biçimlendirme kuralı ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Koşullu biçimlendirme için hücre alanını tanımla
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Zaman dilimi için bir koşul ekle
            int conditionIndex = fcs.AddCondition(FormatConditionType.TimePeriod);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.LightBlue;

            // Zaman dilimi tipini ayarla
            fc.TimePeriod = TimePeriodType.Today;

            // Çalışma kitabını kaydedin
            workbook.Save("TimePeriodTypeExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)



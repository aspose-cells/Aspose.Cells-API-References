---
title: "PivotDateTimeRangeGroupSettings.IsGroupedBy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotDateTimeRangeGroupSettings yöntemi. Alanın tipe göre gruplanıp gruplanmadığını kontrol et"
type: docs
url: /tr/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/isgroupedby/
---
## PivotDateTimeRangeGroupSettings.IsGroupedBy method

Alanının bu türe göre gruplanıp gruplanmadığını kontrol eder.

```csharp
public bool IsGroupedBy(PivotGroupByType type)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | PivotGroupByType | Grup tipi |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDateTimeRangeGroupSettingsMethodIsGroupedByWithPivotGroupByTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Tarihe göre grupla
            PivotField dateField = pivotTable.RowFields[0];
            DateTime start = new DateTime(2023, 1, 1);
            DateTime end = new DateTime(2023, 12, 31);
            dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months }, 1, false);

            // Gruplamayı kontrol et
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            bool isGroupedByMonths = groupSettings.IsGroupedBy(PivotGroupByType.Months);
            
            Console.WriteLine($"Is grouped by months: {isGroupedByMonths}");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



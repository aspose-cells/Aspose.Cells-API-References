---
title: "PivotDateTimeRangeGroupSettings.Interval"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotDateTimeRangeGroupSettings özelliği. Grubun iç değerini alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/
---
## PivotDateTimeRangeGroupSettings.Interval property

Grubun içeriğini alır.

```csharp
public double Interval { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDateTimeRangeGroupSettingsPropertyIntervalDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Örnek veri içeren bir çalışma sayfası ekle
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Örnek tarih verisi ekle
            dataSheet.Cells["A1"].PutValue("Date");
            dataSheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-5));
            dataSheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-4));
            dataSheet.Cells["A4"].PutValue(DateTime.Now.AddDays(-3));
            dataSheet.Cells["A5"].PutValue(DateTime.Now.AddDays(-2));
            dataSheet.Cells["A6"].PutValue(DateTime.Now.AddDays(-1));
            dataSheet.Cells["A7"].PutValue(DateTime.Now);

            // Bir pivot tablo çalışma sayfası ekle
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            
            // Pivot tablo ekle
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:A7", 
                "A1", 
                "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // Tarih alanını satır bölgesine ekleyin
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField dateField = pivotTable.RowFields[0];

            // 2 günlük aralıkla günlere göre grupla
            dateField.GroupBy(1, false);
            PivotDateTimeRangeGroupSettings groupSettings = 
                (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            
            // Interval yalnızca okunabilir olduğundan, gruplama sırasında ayarlamamız gerekir
            // Aralık aslında GroupBy yöntemi parametrelerinde ayarlanır
            // Burada sadece aralık değerini doğruluyoruz
            Console.WriteLine($"Grouping interval: {groupSettings.Interval} days");

            // Çalışma kitabını kaydedin
            workbook.Save("PivotDateTimeGroupingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)



---
title: "TimelineCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TimelineCollection özelliği. Dizine göre Timeline'ı alır"
type: docs
url: /tr/net/aspose.cells.timelines/timelinecollection/item/
---
## TimelineCollection indexer (1 of 2)

Dizine göre Timeline'ı alır.

```csharp
public Timeline this[int index] { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Timelines;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now);
            sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            
            // Önce pivot tablo oluştur
            int pivotIndex = sheet.PivotTables.Add("A1:A3", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // timeline'ı çalışma sayfasına ekle
            int index = sheet.Timelines.Add(pivotTable, 0, 0, "Date");
            
            // Dizine göre Item özelliğini kullanarak timeline'a eriş
            Timeline timelineByIndex = sheet.Timelines[index];
            
            // timeline'ın kullanımını göster
            Console.WriteLine("Timeline name: " + timelineByIndex.Name);
        }
    }
}
```

### Ayrıca Bakınız

* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## TimelineCollection indexer (2 of 2)

Timeline adını kullanarak Timeline'ı alır.

```csharp
public Timeline this[string name] { get; }
```

### Örnekler

```csharp

[C#]

//Timeline adını kullanarak Timeline'ı al.
Timeline objByName = sheet.Timelines["date"];
```

### Ayrıca Bakınız

* class [Timeline](../../timeline/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)



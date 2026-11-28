---
title: "ChartCollection.RemoveAt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartCollection yöntemi. Belirli bir dizindeki grafiği kaldır"
type: docs
url: /tr/net/aspose.cells.charts/chartcollection/removeat/
---
## ChartCollection.RemoveAt method

Belirli bir dizindeki grafiği kaldır.

```csharp
public void RemoveAt(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Grafik indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // İlk grafik sayısını göster
            Console.WriteLine("Initial chart count: " + sheet.Charts.Count);

            // 0. indeksteki grafiği kaldır
            sheet.Charts.RemoveAt(0);

            // Kaldırma sonrası grafik sayısını göster
            Console.WriteLine("Chart count after removal: " + sheet.Charts.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



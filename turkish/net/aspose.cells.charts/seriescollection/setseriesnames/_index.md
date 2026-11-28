---
title: "SeriesCollection.SetSeriesNames"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SeriesCollection yöntemi. Grafikteki tüm serilerin adlarını ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/seriescollection/setseriesnames/
---
## SeriesCollection.SetSeriesNames method

Grafikteki tüm serilerin adlarını ayarlar.

```csharp
public void SetSeriesNames(int startIndex, string area, bool isVertical)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | Int32 | Adını ayarlamak istediğiniz ilk serinin dizini. |
| alan | String | Seri adı için alanı belirtir. |
| isVertical | Boolean | &gt;Seriyi hücre değerleri aralığından satır bazında mı yoksa sütun bazında mı çizeceğini belirtir. |

### Açıklamalar

Başlangıç dizini serilerin sayısından büyükse, işlem geri döner ve hiçbir şey yapmaz. Ardışık hücrelerde veri ayarlanıyorsa, bunları ayırmak için iki nokta üst üste kullanın. Örneğin, $C$2:$C$5. Ardışık hücrelerde veri ayarlanıyorsa, bunları ayırmak için virgül kullanın. Örneğin, ($C$2,$D$5).

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Q1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Q2");
            worksheet.Cells["C2"].PutValue(120);
            worksheet.Cells["C3"].PutValue(180);
            worksheet.Cells["C4"].PutValue(220);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafiğin seri koleksiyonunu al
            SeriesCollection seriesCollection = chart.NSeries;

            try
            {
                // SetSeriesNames'i (startIndex: 0, area: "A2:A4", isVertical: true) parametreleriyle çağır
                seriesCollection.SetSeriesNames(0, "A2:A4", true);

                // Seri verisi ekle
                seriesCollection.Add("B2:C4", true);

                Console.WriteLine("SetSeriesNames method executed successfully with parameters (Int32, String, Boolean)");
                Console.WriteLine("Series names set from range A2:A4");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetSeriesNames method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



---
title: "SeriesCollection.ChangeSeriesOrder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SeriesCollection yöntemi. İki serinin sırasını doğrudan değiştirir"
type: docs
url: /tr/net/aspose.cells.charts/seriescollection/changeseriesorder/
---
## SeriesCollection.ChangeSeriesOrder method

İki serinin sırasını doğrudan değiştirir.

```csharp
[Obsolete("Use SeriesCollection.SwapSeries property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ChangeSeriesOrder(int sourceIndex, int destIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceIndex | Int32 | Geçerli indeks |
| destIndex | Int32 | Hedef indeks |

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen SeriesCollection.SwapSeries yöntemini kullanın. Bu yöntem, Haziran 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodChangeSeriesOrderWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(60);
            
            worksheet.Cells["C1"].PutValue("Series 3");
            worksheet.Cells["C2"].PutValue(70);
            worksheet.Cells["C3"].PutValue(80);
            worksheet.Cells["C4"].PutValue(90);

            // Bir grafik oluştur
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafiğe seri ekle
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            
            // Seri koleksiyonunu alın
            SeriesCollection seriesCollection = chart.NSeries;

            try
            {
                // Seri 0 ve 2'deki serileri değiştirmek için ChangeSeriesOrder yöntemini çağırın
                seriesCollection.ChangeSeriesOrder(0, 2);
                
                Console.WriteLine("Series order changed successfully. Series at index 0 and 2 swapped.");
                
                // Yeni seri sırasını göster
                for (int i = 0; i < seriesCollection.Count; i++)
                {
                    Console.WriteLine($"Series {i + 1}: {seriesCollection[i].Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ChangeSeriesOrder method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("ChangeSeriesOrderWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



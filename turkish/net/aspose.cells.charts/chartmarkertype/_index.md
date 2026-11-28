---
title: "ChartMarkerType enum'ı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.ChartMarkerType enum. Bir çizgi grafiği, dağılım grafiği veya radar grafiğinde işaretçi stilini temsil eder."
type: docs
url: /tr/net/aspose.cells.charts/chartmarkertype/
---
## ChartMarkerType enumeration

Çizgi grafiği, dağılım grafiği veya radar grafiğinde işaretçi stilini temsil eder.

```csharp
public enum ChartMarkerType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Automatic | `0` | Otomatik işaretçiler. |
| Circle | `1` | Dairesel işaretçiler. |
| Dash | `2` | Uzun çubuk işaretçiler |
| Diamond | `3` | Elmas şekilli işaretçiler. |
| Dot | `4` | Kısa çubuk işaretçiler. |
| None | `5` | İşaretçi yok. |
| SquarePlus | `6` | Artı işareti olan kare işaretçiler. |
| Square | `7` | Kare işaretçiler. |
| SquareStar | `8` | Yıldız işareti olan kare işaretçiler. |
| Triangle | `9` | Üçgen işaretçiler. |
| SquareX | `10` | X işaretli kare işaretçiler. |
| Picture | `11` | Resim |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartMarkerTypeDemo
    {
        public static void ChartMarkerTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Veri serisini grafiğe ekle
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk serinin işaretçisine erişin
            Marker marker = chart.NSeries[0].Marker;

            // İşaretçi stilini ayarlayın
            marker.MarkerStyle = ChartMarkerType.Circle;

            // İşaretçi boyutunu ayarlayın
            marker.MarkerSize = 10;

            // İşaretçinin ön plan ve arka plan renklerini ayarlayın
            marker.ForegroundColor = Color.Red;
            marker.BackgroundColor = Color.Yellow;

            // Çalışma kitabını kaydedin
            workbook.Save("ChartMarkerTypeExample.xlsx");
            workbook.Save("ChartMarkerTypeExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)



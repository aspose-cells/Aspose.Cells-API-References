---
title: "Enum DataLabelShapeType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.DataLabelShapeType enum. Bir grafik için kullanılacak önceden ayarlanmış şekil geometrisini belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/datalabelshapetype/
---
## DataLabelShapeType enumeration

Bir grafik için kullanılacak ön ayarlı şekil geometrisini belirtir.

```csharp
public enum DataLabelShapeType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Rect | `0` | Dikdörtgen şekli temsil eder. |
| RoundRect | `1` | Yuvarlak dikdörtgen şekli temsil eder. |
| Ellipse | `2` | Elips şekli temsil eder. |
| RightArrowCallout | `3` | Sağ ok açıklama şekli temsil eder. |
| DownArrowCallout | `4` | Aşağı ok açıklama şekli temsil eder. |
| LeftArrowCallout | `5` | Sol ok açıklama şekli temsil eder. |
| UpArrowCallout | `6` | Yukarı ok açıklama şekli temsil eder. |
| WedgeRectCallout | `7` | Dilimsiz dikdörtgen açıklama şekli temsil eder. |
| WedgeRoundRectCallout | `8` | Dilimsiz yuvarlak dikdörtgen açıklama şekli temsil eder. |
| WedgeEllipseCallout | `9` | Dilimsiz elips açıklama şekli temsil eder. |
| LineCallout | `10` | Çizgi açıklama şekli temsil eder. |
| BentLineCallout | `11` | Bükülmüş çizgi açıklama şekli temsil eder. |
| LineWithAccentBarCallout | `12` | Vurgu çubuğu olan çizgi açıklama şekli temsil eder. |
| BentLineWithAccentBarCallout | `13` | Vurgu çubuğu olan bükülmüş çizgi açıklama şekli temsil eder. |
| Line | `14` | Bu tip yalnızca özel dosya işleme için kullanılır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class DataLabelShapeTypeDemo
    {
        public static void DataLabelShapeTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.SetChartDataRange("A1:B4", true);

            // Grafikteki ilk seriye eriş
            Series series = chart.NSeries[0];

            // Seri için veri etiketlerini etkinleştir
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShapeType = DataLabelShapeType.RoundRect;

            // Çalışma kitabını kaydedin
            workbook.Save("DataLabelShapeTypeExample.xlsx");
            workbook.Save("DataLabelShapeTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



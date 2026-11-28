---
title: "TrendlineCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TrendlineCollection yöntemi. Belirtilen tipte bir Trendline nesnesini bu koleksiyona ekler"
type: docs
url: /tr/net/aspose.cells.charts/trendlinecollection/add/
---
## Add(TrendlineType) {#add}

Belirtilen tipte bir [`Trendline`](../../trendline/) nesnesini bu koleksiyona ekler.

```csharp
public int Add(TrendlineType type)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | TrendlineType | Trendline tipi. |

### Dönüş Değeri

[`Trendline`](../../trendline/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionMethodAddWithTrendlineTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["B4"].PutValue(8);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Seri verisi ekle
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk seriye üstel trendline ekle
            chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);

            // Çalışma kitabını kaydedin
            workbook.Save("TrendlineCollectionMethodAddWithTrendlineTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(TrendlineType, string) {#add_1}

Belirtilen tip ve adla bir [`Trendline`](../../trendline/) nesnesini bu koleksiyona ekler.

```csharp
public int Add(TrendlineType type, string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | TrendlineType | Trendline tipi. |
| name | String | Trendline adı. |

### Dönüş Değeri

[`Trendline`](../../trendline/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionMethodAddWithTrendlineTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // Grafik oluştur
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Seri ekle ve verileri ayarla
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries[0].XValues = "A2:A10";
            chart.NSeries[0].Name = "Data Series";

            // TrendlineType ve ad ile trendline ekle
            chart.NSeries[0].TrendLines.Add(TrendlineType.Logarithmic, "Logarithmic Trend");
            
            // Bazı trendline özelliklerini ayarla
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;
            
            workbook.Save("TrendlineDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



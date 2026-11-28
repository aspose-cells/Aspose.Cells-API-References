---
title: "SeriesCollection.AddR1C1"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SeriesCollection yöntemi. Series koleksiyonunu bir grafiğe ekler"
type: docs
url: /tr/net/aspose.cells.charts/seriescollection/addr1c1/
---
## SeriesCollection.AddR1C1 method

Bir grafiğe [`Series`](../../series/) koleksiyonunu ekler.

```csharp
public int AddR1C1(string area, bool isVertical)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| alan | String | Veri serisini çizecek değerleri belirtir |
| isVertical | Boolean | Seriyi hücre değerleri aralığından satır bazında mı yoksa sütun bazında mı çizeceğini belirtir. |

### Dönüş Değeri

Eklenen ASeries'in NSeries içindeki ilk indeksini döndürür.

### Açıklamalar

Ardışık hücrelerde veri ayarlanıyorsa, bunları ayırmak için iki nokta üst üste kullanın. Örneğin, R[1]C[1]:R[3]C[2]. Ardışık hücrelerde veri ayarlanıyorsa, bunları ayırmak için virgül kullanın. Örneğin, (R[1]C[1],R[3]C[2]).

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddR1C1WithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet wsData = workbook.Worksheets[0];
            wsData.Name = "ChartData";

            // Örnek veri
            wsData.Cells[0, 0].PutValue(1);
            wsData.Cells[1, 0].PutValue(2);
            wsData.Cells[0, 1].PutValue(3);
            wsData.Cells[1, 1].PutValue(4);

            Worksheet wsChart = workbook.Worksheets[workbook.Worksheets.Add(Aspose.Cells.SheetType.Chart)];
            wsChart.Name = "ChartSheet";

            int chartIndex = wsChart.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 0, 0, 15, 15);
            Aspose.Cells.Charts.Chart chart = wsChart.Charts[chartIndex];

            // String ve Boolean parametreleriyle AddR1C1 kullanma
            int seriesIndex = chart.NSeries.AddR1C1("ChartData!R1C2:R2C2", true);
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
            series.XValues = "ChartData!R1C1:R2C1";

            workbook.Save("SeriesCollectionAddR1C1Demo.xlsx", Aspose.Cells.SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



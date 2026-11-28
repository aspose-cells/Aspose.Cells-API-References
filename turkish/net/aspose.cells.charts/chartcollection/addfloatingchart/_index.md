---
title: "ChartCollection.AddFloatingChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartCollection yöntemi. Koleksiyona bir grafik ekler"
type: docs
url: /tr/net/aspose.cells.charts/chartcollection/addfloatingchart/
---
## ChartCollection.AddFloatingChart method

Koleksiyona bir grafik ekler.

```csharp
public int AddFloatingChart(ChartType type, int left, int top, int width, int height)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | ChartType | Grafik türü |
| sol | Int32 | Köşeye x ofseti |
| üst | Int32 | Köşeye y ofseti |
| genişlik | Int32 | Grafik genişliği |
| yükseklik | Int32 | Grafik yüksekliği |

### Dönüş Değeri

[`Chart`](../../chart/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddFloatingChartWithChartTypeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Belirtilen boyutlarla yüzen grafik ekle
            int chartIndex = sheet.Charts.AddFloatingChart(ChartType.Column, 100, 100, 600, 400);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Grafiğe örnek veri ekle
            chart.NSeries.Add("{1,3,2,5}", false);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)



---
title: "Enum WeightType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.WeightType enum. Bir resim kenarı veya bir grafik çizgisi için ağırlık tiplerini listeler."
type: docs
url: /tr/net/aspose.cells.drawing/weighttype/
---
## WeightType enumeration

Bir resim kenarlığı veya grafik çizgisi için ağırlık türlerini listeler.

```csharp
public enum WeightType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| HairLine | `-1` | İnce çizgi ağırlığını temsil eder. |
| MediumLine | `1` | Orta çizgi ağırlığını temsil eder. |
| SingleLine | `0` | Tek çizgi ağırlığını temsil eder. |
| WideLine | `2` | Geniş çizgi ağırlığını temsil eder. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassWeightTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir grafik ekle ve grafik alanını al.
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];
            ChartArea chartArea = chart.ChartArea;
            
            // Kenarlık ağırlık tipini ayarla.
            chartArea.Border.Weight = WeightType.WideLine;
            
            // Ağırlık tipini doğrula.
            Console.WriteLine("Chart Area Border Weight: " + chartArea.Border.Weight);
            
            // Çalışma kitabını kaydedin
            workbook.Save("WeightTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



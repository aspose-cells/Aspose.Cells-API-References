---
title: "Bevel sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Bevel sınıfı. Bir şeklin köşebentini temsil eder."
type: docs
url: /tr/net/aspose.cells.drawing/bevel/
---
## Bevel class

Bir şeklin köşebentini temsil eder

```csharp
public class Bevel
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Height](../../aspose.cells.drawing/bevel/height/) { get; set; } | Köşebentin yüksekliğini alır ve ayarlar, ya da şeklin üzerinde ne kadar yukarı uygulandığını. Birim olarak Nokta kullanılır. |
| [Type](../../aspose.cells.drawing/bevel/type/) { get; set; } | Önceden ayarlanmış köşebent tipini alır ve ayarlar. |
| [Width](../../aspose.cells.drawing/bevel/width/) { get; set; } | Köşebentin genişliğini alır ve ayarlar, ya da şeklin içine ne kadar derine uygulandığını. Birim olarak Nokta kullanılır. |

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class BevelDemo
    {
        public static void RunDemo()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            workbook.CalculateFormula();

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafiğe veri serisi ekle
            chart.NSeries.Add("A1:B4", true);

            // Grafiğin çizim alanına erişin
            ChartFrame plotArea = chart.PlotArea;

            // Çizim alanının şekil özelliklerine erişin
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            // 3B format özelliklerine erişin
            Format3D format3D = shapeProperties.Format3D;

            // Üst köşe özelliklerine erişin
            Bevel topBevel = format3D.TopBevel;

            // Köşebentin genişliğini, yüksekliğini ve tipini ayarlayın
            topBevel.Width = 10.0;
            topBevel.Height = 5.0;
            topBevel.Type = BevelPresetType.Circle;

            // Diğer 3B biçim özelliklerini ayarlayın
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // Çalışma kitabını kaydedin
            workbook.Save("BevelDemo.xlsx");
            workbook.Save("BevelDemo.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



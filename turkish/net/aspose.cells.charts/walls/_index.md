---
title: "Sınıf Walls"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.Walls class. 3B bir grafiğin duvarlarını temsil eden nesneyi kapsüller"
type: docs
url: /tr/net/aspose.cells.charts/walls/
---
## Walls class

3D grafiğin duvarlarını temsil eden nesneyi kapsar.

```csharp
public class Walls : Floor
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Arka plan Rengini alır veya ayarlar [`Area`](../../aspose.cells.drawing/area/). (Şu sınıftan devralınmıştır: [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | Sınırı alır veya ayarlar [`Line`](../../aspose.cells.drawing/line/).(`Floor`'dan devralınmıştır.) |
| [CenterX](../../aspose.cells.charts/walls/centerx/) { get; } | Chart.Calculate() yöntemi çağrıldıktan sonra duvar merkezinin sol-alt köşesinin x koordinatını, grafiğin genişliğinin 1/4000 birimi cinsinden alır. |
| [CenterXPx](../../aspose.cells.charts/walls/centerxpx/) { get; } | Chart.Calculate() yöntemi çağrıldıktan sonra duvar merkezinin sol-alt köşesinin x koordinatını piksel biriminde alır. |
| [CenterY](../../aspose.cells.charts/walls/centery/) { get; } | Chart.Calculate() yöntemi çağrıldıktan sonra duvar merkezinin sol-alt köşesinin y koordinatını, grafiğin yüksekliğinin 1/4000 birimi cinsinden alır. |
| [CenterYPx](../../aspose.cells.charts/walls/centerypx/) { get; } | Chart.Calculate() yöntemi çağrıldıktan sonra duvar merkezinin sol-alt köşesinin y koordinatını piksel biriminde alır. |
| [Depth](../../aspose.cells.charts/walls/depth/) { get; } | Chart.Calculate() yöntemi çağrıldıktan sonra grafiğin genişliğinin 1/4000 birimi cinsinden ön-arkası derinliğini alır. |
| [DepthPx](../../aspose.cells.charts/walls/depthpx/) { get; } | Chart.Calculate() metodunu çağırdıktan sonra ön‑arkaya derinliği piksel biriminde alır. |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Belirtilen grafik veya şekil için doldurma biçimlendirme özelliklerini içeren bir [`FillFormat`](../../aspose.cells.drawing/area/fillformat/) nesnesini temsil eder. (Şu sınıftan devralınmıştır: [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Ön plan Rengini alır veya ayarlar.(Şu sınıftan devralınmıştır: [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Alan biçimlendirmesini temsil eder.(Şu sınıftan devralınmıştır: [`Area`](../../aspose.cells.drawing/area/).) |
| [Height](../../aspose.cells.charts/walls/height/) { get; } | Chart.Calculate() metodunu çağırdıktan sonra üst‑alt yüksekliği, grafiğin yüksekliğinin 1/4000'i biriminde alır. |
| [HeightPx](../../aspose.cells.charts/walls/heightpx/) { get; } | Chart.Calculate() metodunu çağırdıktan sonra üst‑alt yüksekliği piksel biriminde alır. |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Eğer özellik true ise ve grafik noktasının değeri negatif bir sayıysa, ön plan rengi ve arka plan rengi değiştirilecektir.(Şu sınıftan devralınmıştır: [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Alan şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar.(Şu sınıftan devralınmıştır: [`Area`](../../aspose.cells.drawing/area/).) |
| [Width](../../aspose.cells.charts/walls/width/) { get; } | Chart.Calculate() metodunu çağırdıktan sonra sol‑sağ genişliği, grafiğin genişliğinin 1/4000'i biriminde alır. |
| [WidthPx](../../aspose.cells.charts/walls/widthpx/) { get; } | Chart.Calculate() metodunu çağırdıktan sonra sol‑sağ genişliği piksel biriminde alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetCubePointCount](../../aspose.cells.charts/walls/getcubepointcount/)() | Chart.Calculate() metodunu çağırdıktan sonra küp noktalarının sayısını alır. |
| [GetCubePointXPx](../../aspose.cells.charts/walls/getcubepointxpx/)(int) | Chart.Calculate() metodunu çağırdıktan sonra duvar küpünün tepe noktasının x koordinatını alır. Duvar küpünün tepe noktası sayısı sekizdir |
| [GetCubePointYPx](../../aspose.cells.charts/walls/getcubepointypx/)(int) | Chart.Calculate() metodunu çağırdıktan sonra duvar küpünün tepe noktasının y koordinatını alır. Duvar küpünün tepe noktası sayısı sekizdir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class WallsDemo
    {
        public static void WallsExample()
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

            // Çalışma sayfasına bir 3D grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafiği hesaplayarak özelliklerini güncelle
            chart.Calculate();

            // 3D grafiğin duvarlarına eriş
            Walls walls = chart.Walls;

            // Duvarların özelliklerini ayarla
            walls.BackgroundColor = Color.LightBlue;
            walls.ForegroundColor = Color.DarkBlue;
            walls.Formatting = FormattingType.Custom;
            walls.InvertIfNegative = true;
            walls.Transparency = 0.5;

            // Duvarların kenarına eriş ve özelliklerini ayarla
            Line border = walls.Border;
            border.Color = Color.Red;
            border.Style = LineType.Solid;

            // Duvarların bazı özelliklerini yazdır
            Console.WriteLine("CenterX: " + walls.CenterX);
            Console.WriteLine("CenterY: " + walls.CenterY);
            Console.WriteLine("Width: " + walls.Width);
            Console.WriteLine("Depth: " + walls.Depth);
            Console.WriteLine("Height: " + walls.Height);
            Console.WriteLine("CenterXPx: " + walls.CenterXPx);
            Console.WriteLine("CenterYPx: " + walls.CenterYPx);
            Console.WriteLine("WidthPx: " + walls.WidthPx);
            Console.WriteLine("DepthPx: " + walls.DepthPx);
            Console.WriteLine("HeightPx: " + walls.HeightPx);

            // Çalışma kitabını kaydedin
            workbook.Save("WallsExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Floor](../floor/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)



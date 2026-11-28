---
title: "Sınıf Floor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.Floor sınıfı. 3D grafiğin tabanını temsil eden nesneyi kapsüller"
type: docs
url: /tr/net/aspose.cells.charts/floor/
---
## Floor class

3D bir grafiğin tabanını temsil eden nesneyi kapsar.

```csharp
public class Floor : Area
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Arka plan Rengini alır veya ayarlar [`Area`](../../aspose.cells.drawing/area/). (Şu sınıftan devralınmıştır: [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | Kenarı alır veya ayarlar [`Line`](../../aspose.cells.drawing/line/). |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Belirtilen grafik veya şekil için doldurma biçimlendirme özelliklerini içeren bir [`FillFormat`](../../aspose.cells.drawing/area/fillformat/) nesnesini temsil eder. (Şu sınıftan devralınmıştır: [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Ön plan Rengini alır veya ayarlar.(Şu sınıftan devralınmıştır: [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Alan biçimlendirmesini temsil eder.(Şu sınıftan devralınmıştır: [`Area`](../../aspose.cells.drawing/area/).) |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Eğer özellik true ise ve grafik noktasının değeri negatif bir sayıysa, ön plan rengi ve arka plan rengi değiştirilecektir.(Şu sınıftan devralınmıştır: [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Alan şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar.(Şu sınıftan devralınmıştır: [`Area`](../../aspose.cells.drawing/area/).) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FloorDemo
    {
        public static void FloorExample()
        {
            // Çalışma kitabı nesnesini örnekle
            Workbook workbook = new Workbook();

            // Hücre koleksiyonunu al
            Cells cells = workbook.Worksheets[0].Cells;

            // Hücrelere değerleri koy
            cells["A1"].PutValue(1);
            cells["A2"].PutValue(2);
            cells["A3"].PutValue(3);

            // Grafik koleksiyonunu al
            ChartCollection charts = workbook.Worksheets[0].Charts;

            // Yeni bir grafik ekle
            int index = charts.Add(ChartType.Column3DStacked, 5, 0, 15, 5);

            // Yeni eklenen grafiği al
            Chart chart = charts[index];

            // Grafiğin nseries'ını ayarla
            chart.NSeries.Add("A1:A3", true);

            // Veri etiketlerini göster
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Grafiğin tabanını al
            Floor floor = chart.Floor;

            // Tabanın kenarlığını kırmızı olarak ayarla
            floor.Border.Color = Color.Red;

            // Dolgu biçimini ayarla
            floor.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.DiagonalDown, 2);

            // Ek özellikleri ayarla
            floor.BackgroundColor = Color.LightBlue;
            floor.ForegroundColor = Color.DarkBlue;
            floor.Formatting = FormattingType.Custom;
            floor.InvertIfNegative = true;
            floor.Transparency = 0.5;

            // Dosyayı kaydet
            workbook.Save(@"FloorExample.xlsx");
            workbook.Save(@"FloorExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* class [Area](../../aspose.cells.drawing/area/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)



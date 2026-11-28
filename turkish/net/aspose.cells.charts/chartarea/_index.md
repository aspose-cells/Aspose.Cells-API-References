---
title: "Sınıf ChartArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.ChartArea sınıfı. Çalışma sayfasındaki grafik alanını temsil eden nesneyi kapsar."
type: docs
url: /tr/net/aspose.cells.charts/chartarea/
---
## ChartArea class

Çalışma sayfasındaki grafik alanını temsil eden nesneyi kapsar.

```csharp
public class ChartArea : ChartFrame
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area/) { get; } | Alır [`area`](../chartframe/area/).(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont/) { get; set; } | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa True. Varsayılan değer True'dir.(Inherited from [`ChartFrame`](../chartframe/).) |
| [Background](../../aspose.cells.charts/chartframe/background/) { get; set; } | (**Obsolete.**) Arka planın görüntüleme modunu alır ve ayarlar. Bu özellik yalnızca Excel 2003 veya daha eski sürümlerde geçerlidir.(Inherited from [`ChartFrame`](../chartframe/).) |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode/) { get; set; } | (**Obsolete.**) Arka planın görüntüleme modunu alır ve ayarlar. Bu özellik yalnızca Excel 2003 veya daha eski sürümlerde geçerlidir.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [Border](../../aspose.cells.charts/chartframe/border/) { get; } | Alır [`border`](../../aspose.cells.drawing/line/).(Inherited from [`ChartFrame`](../chartframe/).) |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight/) { get; } | (**Obsolete.**) Varsayılan konumun yüksekliğini, grafik alanının 1/4000 birimi cinsinden temsil eder.(Inherited from [`ChartFrame`](../chartframe/).) |
| [DefaultHeightRatioToChart](../../aspose.cells.charts/chartframe/defaultheightratiotochart/) { get; } | Varsayılan konumun yüksekliğini, grafik alanının kesir birimi cinsinden temsil eder.(Inherited from [`ChartFrame`](../chartframe/).) |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth/) { get; } | (**Obsolete.**) Varsayılan konumun genişliğini, grafik alanının 1/4000 birimi cinsinden temsil eder.(Inherited from [`ChartFrame`](../chartframe/).) |
| [DefaultWidthRatioToChart](../../aspose.cells.charts/chartframe/defaultwidthratiotochart/) { get; } | Varsayılan konumun genişliğini, grafik alanının kesir birimi cinsinden temsil eder.(Inherited from [`ChartFrame`](../chartframe/).) |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx/) { get; } | (**Obsolete.**) Varsayılan konumun x koordinatını, grafik alanının 1/4000 birimi cinsinden temsil eder.(Inherited from [`ChartFrame`](../chartframe/).) |
| [DefaultXRatioToChart](../../aspose.cells.charts/chartframe/defaultxratiotochart/) { get; } | Varsayılan konumun x koordinatını, grafik alanının kesir birimi cinsinden temsil eder.(Inherited from [`ChartFrame`](../chartframe/).) |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty/) { get; } | (**Obsolete.**) Varsayılan konumun y koordinatını, grafik alanının 1/4000 birimi cinsinden temsil eder.(Inherited from [`ChartFrame`](../chartframe/).) |
| [DefaultYRatioToChart](../../aspose.cells.charts/chartframe/defaultyratiotochart/) { get; } | Varsayılan konumun y koordinatını, grafik alanının kesir birimi cinsinden temsil eder.(Inherited from [`ChartFrame`](../chartframe/).) |
| override [Font](../../aspose.cells.charts/chartarea/font/) { get; } | Belirtilen ChartArea nesnesinin bir [`Font`](./font/) nesnesini alır. |
| override [Height](../../aspose.cells.charts/chartarea/height/) { get; set; } | (**Obsolete.**) Grafik alanının alt‑sağ köşe satırından dikey ofseti alır veya ayarlar, grafik alanının 1/4000 birimi olarak. |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | Çerçevenin yüksekliğini piksel biriminde alır veya ayarlar.(Inherited from [`ChartFrame`](../chartframe/).) |
| override [HeightRatioToChart](../../aspose.cells.charts/chartarea/heightratiotochart/) { get; set; } | Grafik alanının alt sağ köşe satırından dikey ofseti alır veya ayarlar, grafik alanının oran birimi olarak. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | Grafik çerçevesinin otomatik boyutlandırılıp boyutlandırılmadığını gösterir.(Inherited from [`ChartFrame`](../chartframe/).) |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | Varsayılan konumun (DefaultX, DefaultY, DefaultWidth ve DefaultHeight) ayarlanıp ayarlanmadığını gösterir.(Inherited from [`ChartFrame`](../chartframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | Çizim alanı boyutunun tik işaretlerini ve eksen etiketlerini içerip içermediğini gösterir. False, boyutun çizim alanı, tik işaretleri ve eksen etiketlerinin boyutunu belirleyeceğini belirtir.(Inherited from [`ChartFrame`](../chartframe/).) |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | Çerçevenin gölgesi varsa True.(Inherited from [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | `[`ShapeProperties`](../chartframe/shapeproperties/)` nesnesini alır.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont/) { get; } | (**Obsolete.**) Belirtilen ChartFrame nesnesinin bir [`Font`](../chartframe/font/) nesnesini alır.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions/) { get; } | Metnin seçeneklerini alır ve ayarlar.(Inherited from [`ChartFrame`](../chartframe/).) |
| override [Width](../../aspose.cells.charts/chartarea/width/) { get; set; } | (**Obsolete.**) Grafik alanının alt sağ köşe sütunundan yatay ofseti alır veya ayarlar, grafik alanının 1/4000 birimi olarak. |
| virtual [WidthPixel](../../aspose.cells.charts/chartframe/widthpixel/) { get; set; } | Çerçevenin genişliğini piksel birimi cinsinden alır veya ayarlar.([`ChartFrame`](../chartframe/) üzerinden devralınmıştır.) |
| override [WidthRatioToChart](../../aspose.cells.charts/chartarea/widthratiotochart/) { get; set; } | Grafik alanının alt sağ köşe sütunundan yatay ofseti alır veya ayarlar, grafik alanının oran birimi olarak. |
| override [X](../../aspose.cells.charts/chartarea/x/) { get; set; } | (**Obsolete.**) Grafik alanının üst‑sol köşe sütunundan yatay ofseti alır veya ayarlar, grafik alanının 1/4000 birimi olarak. |
| virtual [XPixel](../../aspose.cells.charts/chartframe/xpixel/) { get; set; } | Üst sol köşenin x koordinatını piksel birimi cinsinden alır veya ayarlar.([`ChartFrame`](../chartframe/) üzerinden devralınmıştır.) |
| override [XRatioToChart](../../aspose.cells.charts/chartarea/xratiotochart/) { get; set; } | Grafik alanının üst‑sol köşe sütunundan yatay ofseti alır veya ayarlar, grafik alanının oranı olarak. |
| override [Y](../../aspose.cells.charts/chartarea/y/) { get; set; } | (**Obsolete.**) Grafik alanının üst sol köşe satırından dikey ofseti alır veya alır, grafik alanının 1/4000 birimi olarak. |
| virtual [YPixel](../../aspose.cells.charts/chartframe/ypixel/) { get; set; } | Üst sol köşenin y koordinatını piksel birimi cinsinden alır veya ayarlar.([`ChartFrame`](../chartframe/) üzerinden devralınmıştır.) |
| override [YRatioToChart](../../aspose.cells.charts/chartarea/yratiotochart/) { get; set; } | Grafik alanının üst sol köşe satırından dikey ofseti alır veya alır, grafik alanının oran birimi olarak. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | Çerçevenin konumunu otomatik olarak ayarla.([`ChartFrame`](../chartframe/) üzerinden devralınmıştır.) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartAreaDemo
    {
        public static void ChartAreaExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasının referansını elde etme
            Worksheet worksheet = workbook.Worksheets[0];

            // \"A1\" hücresine örnek bir değer ekleniyor
            worksheet.Cells["A1"].PutValue(50);

            // \"A2\" hücresine örnek bir değer ekleniyor
            worksheet.Cells["A2"].PutValue(100);

            // \"A3\" hücresine örnek bir değer ekleniyor
            worksheet.Cells["A3"].PutValue(150);

            // \"B1\" hücresine örnek bir değer ekleniyor
            worksheet.Cells["B1"].PutValue(60);

            // \"B2\" hücresine örnek bir değer ekleniyor
            worksheet.Cells["B2"].PutValue(32);

            // \"B3\" hücresine örnek bir değer ekleniyor
            worksheet.Cells["B3"].PutValue(50);

            // Çalışma sayfasına bir grafik ekleme
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);

            // Yeni eklenen grafiğin örneğine erişme
            Chart chart = worksheet.Charts[chartIndex];

            // Grafiğe, "A1" hücresinden "B3" hücresine kadar uzanan NSeries (grafik veri kaynağı) ekleniyor
            chart.NSeries.Add("A1:B3", true);

            // Grafik Alanını Alma
            ChartArea chartArea = chart.ChartArea;

            // ChartArea özelliklerini ayarlama
            chartArea.X = 10;
            chartArea.Y = 10;
            chartArea.Width = 400;
            chartArea.Height = 300;
            chartArea.IsInnerMode = false;
            chartArea.AutoScaleFont = true;
            chartArea.BackgroundMode = BackgroundMode.Transparent;
            chartArea.IsAutomaticSize = true;
            chartArea.Shadow = true;

            // Şema alanının ön plan rengini ayarlama
            chartArea.Area.ForegroundColor = Color.Yellow;

            // Excel dosyasını kaydetme
            workbook.Save("ChartAreaExample.xlsx");
            workbook.Save("ChartAreaExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartFrame](../chartframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)



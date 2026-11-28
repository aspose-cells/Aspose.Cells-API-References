---
title: "Sınıf Line"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Line sınıfı. Çizgi biçimini temsil eden nesneyi kapsüller"
type: docs
url: /tr/net/aspose.cells.drawing/line/
---
## Line class

Çizgi biçimini temsil eden nesneyi kapsüller.

```csharp
public class Line
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | Bir çizginin başlangıcı için ok başının uzunluğunu belirtir. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | Bir çizginin başlangıcı için ok başının genişliğini belirtir. |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | Bir çizginin başlangıcı için ok başı belirtir. |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | Bitiş kapaklarını belirtir. |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | Çizginin Rengini temsil eder. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | Bileşik çizgi tipini belirtir |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | Kesikli çizgi tipini belirtir |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | Bir çizginin sonu için ok başının uzunluğunu belirtir. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | Bir çizginin sonu için ok başının genişliğini belirtir. |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | Bir çizginin sonu için ok başı belirtir. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | Biçim tipini alır veya ayarlar. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | Gradyan doldurmayı temsil eder. |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | Bu çizgi stilinin otomatik atanıp atanmadığını gösterir. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | Çizgi renginin otomatik atanıp atanmadığını gösterir. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | Çizginin görünür olup olmadığını temsil eder. |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | Birleştirme uçlarını belirtir. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | Çizgi stilini temsil eder. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | Tema rengini alır ve ayarlar. |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | Çizginin şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak alır veya ayarlar. |
| [Weight](../../aspose.cells.drawing/line/weight/) { get; set; } | Çizginin [`WeightType`](../weighttype/) değerini alır veya ayarlar. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt/) { get; set; } | Çizginin ağırlığını puan biriminde alır veya ayarlar. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx/) { get; set; } | Çizginin ağırlığını piksel biriminde alır veya ayarlar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassLineDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Cells cells = sheet.Cells;
            cells[0,1].PutValue("Income");
            cells[1,0].PutValue("Company A");
            cells[2,0].PutValue("Company B");
            cells[3,0].PutValue("Company C");
            cells[1,1].PutValue(10000);
            cells[2,1].PutValue(20000);
            cells[3,1].PutValue(30000);
            
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 9, 9, 21, 15);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            chart.NSeries.Add("B1:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            chart.NSeries[0].Border.Style = LineType.Dot;
            chart.NSeries[0].Border.Color = Color.Red;
            chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Triangle;
            chart.NSeries[0].Border.Weight = WeightType.MediumLine;
            
            workbook.Save("LineChartDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)



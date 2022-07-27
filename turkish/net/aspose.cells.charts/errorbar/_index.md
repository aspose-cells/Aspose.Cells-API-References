---
title: ErrorBar
second_title: Aspose.Cells for .NET API Referansı
description: Veri serisinin hata çubuğunu temsil eder.
type: docs
weight: 630
url: /tr/net/aspose.cells.charts/errorbar/
---
## ErrorBar class

Veri serisinin hata çubuğunu temsil eder.

```csharp
public class ErrorBar : Line
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Amount](../../aspose.cells.charts/errorbar/amount) { get; set; } | Hata çubuğunun miktarını temsil eder.  Tutar sıfırdan büyük veya sıfıra eşit olmalıdır. |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Bir satırın başlangıcı için ok ucunun uzunluğunu belirtir. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Bir satırın başlangıcı için ok ucunun genişliğini belirtir. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Bir satırın başlangıcı için bir ok başı belirtir. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Bitiş büyük harflerini belirtir. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | Color satırın. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Bileşik satır türünü belirtir |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Kısa çizgi tipini belirtir |
| [DisplayType](../../aspose.cells.charts/errorbar/displaytype) { get; set; } | Hata çubuğu görüntüleme türünü temsil eder. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Bir satırın sonu için ok ucunun uzunluğunu belirtir. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Bir satırın sonu için ok ucunun genişliğini belirtir. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Bir satırın sonu için bir ok başı belirtir. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Biçim türünü alır veya ayarlar. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Degrade dolguyu temsil eder. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Bu çizgi stilinin otomatik olarak atanıp atanmadığını gösterir. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Çizgi renginin otomatik olarak atanıp atanmadığını gösterir. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Çizginin görünür olup olmadığını temsil eder. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Birleştirme büyük harflerini belirtir. |
| [MinusValue](../../aspose.cells.charts/errorbar/minusvalue) { get; set; } | Hata çubuğu türü Özel olduğunda negatif hata miktarını temsil eder. |
| [PlusValue](../../aspose.cells.charts/errorbar/plusvalue) { get; set; } | Hata çubuğu türü Özel olduğunda pozitif hata miktarını temsil eder. |
| [ShowMarkerTTop](../../aspose.cells.charts/errorbar/showmarkerttop) { get; set; } | Hata çubuklarının bir T-top ile biçimlendirilip biçimlendirilmediğini gösterir. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Çizginin stilini temsil eder. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Tema rengini alır ve ayarlar. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Çizginin şeffaflık derecesini 0.0 (opak) ile 1.0 (net) arasında bir değer olarak döndürür veya ayarlar. |
| [Type](../../aspose.cells.charts/errorbar/type) { get; set; } | Hata çubuğu tutar türünü temsil eder. |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Alır veya ayarlar[`WeightType`](../../aspose.cells.drawing/weighttype) satırın. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Çizginin ağırlığını puan birimi cinsinden alır veya ayarlar. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Çizginin ağırlığını piksel birimi cinsinden alır veya ayarlar. |

### Örnekler

```csharp
[C#]
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["a1"].PutValue(2);
cells["a2"].PutValue(5);
cells["a3"].PutValue(3);
cells["a4"].PutValue(6);
cells["b1"].PutValue(4);
cells["b2"].PutValue(3);
cells["b3"].PutValue(6);
cells["b4"].PutValue(7);

cells["C1"].PutValue("Q1");
cells["C2"].PutValue("Q2");
cells["C3"].PutValue("Y1");
cells["C4"].PutValue("Y2");

int chartIndex = excel.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);

Chart chart = excel.Worksheets[0].Charts[chartIndex];
chart.NSeries.Add("A1:B4", true);

chart.NSeries.CategoryData = "C1:C4";

for(int i = 0; i < chart.NSeries.Count; i ++)
{
	ASeries aseries = chart.NSeries[i];
	aseries.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
	aseries.YErrorBar.Type = ErrorBarType.FixedValue;
	aseries.YErrorBar.Amount = 5;
}

[Visual Basic]
Dim workbook As Workbook =  New Workbook() 
Dim cells As Cells =  workbook.Worksheets(0).Cells 
cells("a1").PutValue(2)
cells("a2").PutValue(5)
cells("a3").PutValue(3)
cells("a4").PutValue(6)
cells("b1").PutValue(4)
cells("b2").PutValue(3)
cells("b3").PutValue(6)
cells("b4").PutValue(7)

cells("C1").PutValue("Q1")
cells("C2").PutValue("Q2")
cells("C3").PutValue("Y1")
cells("C4").PutValue("Y2")

Dim chartIndex As Integer =  excel.Worksheets(0).Charts.Add(ChartType.Column,11,0,27,10) 

Dim chart As Chart =  excel.Worksheets(0).Charts(chartIndex) 
chart.NSeries.Add("A1:B4", True)

chart.NSeries.CategoryData = "C1:C4"

Dim i As Integer
For  i = 0 To chart.NSeries.Count - 1
Dim aseries As ASeries =  chart.NSeries(i) 
aseries.YErrorBar.DisplayType = ErrorBarDisplayType.Minus
aseries.YErrorBar.Type = ErrorBarType.FixedValue
aseries.YErrorBar.Amount = 5
Next
```

### Ayrıca bakınız

* class [Line](../../aspose.cells.drawing/line)
* ad alanı [Aspose.Cells.Charts](../../aspose.cells.charts)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

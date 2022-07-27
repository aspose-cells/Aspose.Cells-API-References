---
title: Legend
second_title: Aspose.Cells for .NET API Referansı
description: Grafik göstergesini temsil eden nesneyi kapsüller.
type: docs
weight: 690
url: /tr/net/aspose.cells.charts/legend/
---
## Legend class

Grafik göstergesini temsil eden nesneyi kapsüller.

```csharp
public class Legend : ChartTextFrame
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | [`alan`](../chartframe/area) . |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | Nesne boyutu değiştiğinde nesnedeki metin yazı tipi boyutunu değiştirirse doğrudur. Varsayılan değer True'dur. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | background öğesinin görüntüleme modunu alır ve ayarlar |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | [`sınır`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Varsayılan konumun yüksekliğini temsil eder |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Varsayılan konumun genişliğini temsil eder |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Varsayılan konumun x'ini temsil eder |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Varsayılan konumun y'sini temsil eder |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Metnin yönünü alır ve ayarlar. |
| virtual [Font](../../aspose.cells.charts/chartframe/font) { get; } | [`Font`](../chartframe/font) belirtilen ChartFrame nesnesinin nesnesi. |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Grafik alanının 1/4000 biriminde çerçevenin yüksekliğini alır veya ayarlar. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Grafik çerçevesinin otomatik boyutlu olup olmadığını gösterir. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Metnin otomatik olarak oluşturulduğunu gösterir. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Varsayılan konumun (DefaultX, DefaultY, DefaultWidth ve DefaultHeight) ayarlanıp ayarlanmadığını gösterir. |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Bu veri etiketlerinin silinip silinmediğini gösterir. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Çizim alanı boyutunun onay işaretlerini ve eksen etiketlerini içerip içermediğini gösterir. False, boyutun çizim alanının boyutunu, onay işaretlerini ve eksen etiketlerini belirleyeceğini belirtir. |
| [IsOverLay](../../aspose.cells.charts/legend/isoverlay) { get; set; } | Diğer grafik öğelerinin bu grafik öğesiyle çakışmasına izin verilip verilmeyeceğini alır veya ayarlar. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Bir şeklin, içinde açıklanan metni tam olarak içermesi için otomatik olarak sığdırılıp sığdırılmaması gerektiğini alır veya ayarlar. Bir şeklin içindeki metin, içindeki tüm metni içerecek şekilde ölçeklendiğinde otomatik sığdırma olur. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Metnin sarılıp sarılmadığını belirten bir değer alır veya ayarlar. |
| [LegendEntries](../../aspose.cells.charts/legend/legendentries) { get; } | Belirtilen grafik göstergesindeki tüm LegendEntry nesnelerinin bir koleksiyonunu alır. Yüzey grafiğinin gösterge girişlerinin ayarlanması desteklenmez. Dolayısıyla, grafik türü yüzey grafiği türü ise null döndürür. |
| [LegendEntriesLabels](../../aspose.cells.charts/legend/legendentrieslabels) { get; } | Chart.Calculate() yöntemini çağırdıktan sonra gösterge girişlerinin etiketlerini alır. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Çalışma sayfasına bir başvuru alır ve ayarlar. |
| [Position](../../aspose.cells.charts/legend/position) { get; set; } | Gösterge konum türünü alır veya ayarlar. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Metin okuma sırasını temsil eder. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Metin döndürme açısını temsil eder. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Çerçevenin gölgesi varsa doğrudur. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | [`ShapeProperties`](../chartframe/shapeproperties) nesne. |
| virtual [Text](../../aspose.cells.charts/charttextframe/text) { get; set; } | Çerçeve başlığının metnini alır veya ayarlar. |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | Metni yatay hizalamayı alır ve ayarlar. |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | Metnin dikey hizalamasını alır veya ayarlar. |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | Grafik alanının 1/4000 biriminde çerçevenin genişliğini alır veya ayarlar. |
| virtual [X](../../aspose.cells.charts/chartframe/x) { get; set; } | Grafik alanının 1/4000 biriminde sol üst köşenin x koordinatını alır veya ayarlar. |
| virtual [Y](../../aspose.cells.charts/chartframe/y) { get; set; } | Grafik alanının 1/4000 biriminde sol üst köşenin y koordinatını alır veya ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | Metin içindeki bir dizi karakteri temsil eden bir Karakterler nesnesi döndürür. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Çerçevenin konumunu otomatik olarak ayarlayın |

### Örnekler

```csharp
[C#]
   
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
		
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
// Efsanenin genişliğini ve yüksekliğini ayarla
Legend legend = chart.Legend;

//Efsane varsayılan olarak grafiğin sağ tarafındadır.
//Lejand grafiğin solunda veya sağındaysa, Legend.X özelliğinin ayarlanması etkili olmaz.
//Lejand grafiğin üst veya alt tarafındaysa, Legend.Y özelliğinin ayarlanması etkili olmaz.
legend.Y = 1500;
legend.Width = 50;
legend.Height = 50; 
// Efsanenin konumunu ayarla
legend.Position = LegendPositionType.Left;

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)

Dim chart as Chart = sheet.Charts(chartIndex)
chart.SetChartDataRange("A1:B4", True);
 
'Set Legend's width and height
Dim legend as Legend = chart.Legend

'Gösterge, varsayılan olarak grafiğin sağ tarafındadır.
'Gösterge grafiğin solunda veya sağındaysa, Legend.X özelliğinin ayarlanması etkili olmaz.
'Gösterge grafiğin üst veya alt tarafındaysa, Legend.Y özelliğinin ayarlanması etkili olmaz.
legend.Y = 1500
legend.Width = 50
legend.Height = 50
'Set legend's position
legend.Position = LegendPositionType.Left
```

### Ayrıca bakınız

* class [ChartTextFrame](../charttextframe)
* ad alanı [Aspose.Cells.Charts](../../aspose.cells.charts)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

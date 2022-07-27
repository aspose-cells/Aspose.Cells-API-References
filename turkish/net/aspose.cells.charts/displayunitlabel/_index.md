---
title: DisplayUnitLabel
second_title: Aspose.Cells for .NET API Referansı
description: Görüntü birimi etiketini temsil eder.
type: docs
weight: 600
url: /tr/net/aspose.cells.charts/displayunitlabel/
---
## DisplayUnitLabel class

Görüntü birimi etiketini temsil eder.

```csharp
public class DisplayUnitLabel : ChartTextFrame
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | [`alan`](../chartframe/area) . |
| override [AutoScaleFont](../../aspose.cells.charts/displayunitlabel/autoscalefont) { get; set; } | Nesne boyutu değiştiğinde nesnedeki metin yazı tipi boyutunu değiştirirse doğrudur. Varsayılan değer True'dur. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | background öğesinin görüntüleme modunu alır ve ayarlar |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | [`sınır`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Varsayılan konumun yüksekliğini temsil eder |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Varsayılan konumun genişliğini temsil eder |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Varsayılan konumun x'ini temsil eder |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Varsayılan konumun y'sini temsil eder |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Metnin yönünü alır ve ayarlar. |
| override [Font](../../aspose.cells.charts/displayunitlabel/font) { get; } | [`Font`](./font) belirtilen ChartFrame nesnesinin nesnesi. |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Grafik alanının 1/4000 biriminde çerçevenin yüksekliğini alır veya ayarlar. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Grafik çerçevesinin otomatik boyutlu olup olmadığını gösterir. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Metnin otomatik olarak oluşturulduğunu gösterir. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Varsayılan konumun (DefaultX, DefaultY, DefaultWidth ve DefaultHeight) ayarlanıp ayarlanmadığını gösterir. |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Bu veri etiketlerinin silinip silinmediğini gösterir. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Çizim alanı boyutunun onay işaretlerini ve eksen etiketlerini içerip içermediğini gösterir. False, boyutun çizim alanının boyutunu, onay işaretlerini ve eksen etiketlerini belirleyeceğini belirtir. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Bir şeklin, içinde açıklanan metni tam olarak içermesi için otomatik olarak sığdırılıp sığdırılmaması gerektiğini alır veya ayarlar. Bir şeklin içindeki metin, içindeki tüm metni içerecek şekilde ölçeklendiğinde otomatik sığdırma olur. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Metnin sarılıp sarılmadığını belirten bir değer alır veya ayarlar. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Çalışma sayfasına bir başvuru alır ve ayarlar. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Metin okuma sırasını temsil eder. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Metin döndürme açısını temsil eder. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Çerçevenin gölgesi varsa doğrudur. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | [`ShapeProperties`](../chartframe/shapeproperties) nesne. |
| override [Text](../../aspose.cells.charts/displayunitlabel/text) { get; set; } | Görüntü birimi etiketinin metnini alır veya ayarlar. |
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

//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();
//Excel nesnesine yeni bir çalışma sayfası ekleme
int sheetIndex = workbook.Worksheets.Add();
//Yeni eklenen çalışma sayfasının sayfa indeksini geçerek referansının alınması
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//"A1" hücresine örnek değer ekleme
worksheet.Cells["A1"].PutValue(50);
//"A2" hücresine örnek değer ekleme
worksheet.Cells["A2"].PutValue(100);
//"A3" hücresine örnek değer ekleme
worksheet.Cells["A3"].PutValue(150);
//"A4" hücresine örnek değer ekleme
worksheet.Cells["A4"].PutValue(200);
//"B1" hücresine örnek değer ekleme
worksheet.Cells["B1"].PutValue(60);
//"B2" hücresine örnek değer ekleme
worksheet.Cells["B2"].PutValue(32);
//"B3" hücresine örnek değer ekleme
worksheet.Cells["B3"].PutValue(50);
//"B4" hücresine örnek değer ekleme
worksheet.Cells["B4"].PutValue(40);
//"C1" hücresine kategori verisi olarak örnek değer ekleme
worksheet.Cells["C1"].PutValue("Q1");
//"C2" hücresine kategori verisi olarak örnek değer ekleme
worksheet.Cells["C2"].PutValue("Q2");
//"C3" hücresine kategori verisi olarak örnek değer ekleme
worksheet.Cells["C3"].PutValue("Y1");
//"C4" hücresine kategori verisi olarak örnek değer ekleme
worksheet.Cells["C4"].PutValue("Y2");
//Çalışma sayfasına grafik ekleme
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Yeni eklenen grafiğin örneğine erişim
Chart chart = worksheet.Charts[chartIndex];
//"A1" hücresinden "B4"e kadar olan grafiğe NSeries (grafik veri kaynağı) ekleme
chart.NSeries.Add("A1:B4", true);
// NSeries'in kategori verileri için veri kaynağının ayarlanması
chart.NSeries.CategoryData = "C1:C4";
//değer(Y) ekseninin gösterim birimini ayarlama.
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;
//Özel görüntüleme birimi etiketinin ayarlanması
displayUnitLabel.Text = "100";
//Excel dosyasını kaydetme
workbook.Save("book1.xls");

[Visual Basic]

'Bir Çalışma Kitabı nesnesini başlatma
Dim workbook As Workbook = New Workbook()
'Excel nesnesine yeni bir çalışma sayfası ekleme
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Yeni eklenen çalışma sayfasının sayfa indeksini geçerek referansını alma
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'Çalışma sayfasına grafik ekleme
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Yeni eklenen grafiğin örneğine erişme
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", True)
'NSeries kategori verileri için veri kaynağını ayarlama
Chart.NSeries.CategoryData = "C1:C4"
'Değer(Y) ekseninin görüntü birimini ayarlama.
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds
Dim displayUnitLabel As DisplayUnitLabel = chart.ValueAxis.DisplayUnitLabel
'Özel ekran birimi etiketini ayarlama
displayUnitLabel.Text = "100"
'Excel dosyasını kaydetme
workbook.Save("book1.xls")
```

### Ayrıca bakınız

* class [ChartTextFrame](../charttextframe)
* ad alanı [Aspose.Cells.Charts](../../aspose.cells.charts)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

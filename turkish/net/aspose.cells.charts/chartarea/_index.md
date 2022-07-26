---
title: ChartArea
second_title: Aspose.Cells for .NET API Referansı
description: Çalışma sayfasındaki grafik alanını temsil eden nesneyi kapsüller.
type: docs
weight: 440
url: /tr/net/aspose.cells.charts/chartarea/
---
## ChartArea class

Çalışma sayfasındaki grafik alanını temsil eden nesneyi kapsüller.

```csharp
public class ChartArea : ChartFrame
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
| override [Font](../../aspose.cells.charts/chartarea/font) { get; } | [`Font`](./font) belirtilen chartarea nesnesinin nesnesi. |
| override [Height](../../aspose.cells.charts/chartarea/height) { get; set; } | Sağ alt köşe satırından dikey ofseti alır veya ayarlar. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Grafik çerçevesinin otomatik boyutlu olup olmadığını gösterir. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Varsayılan konumun (DefaultX, DefaultY, DefaultWidth ve DefaultHeight) ayarlanıp ayarlanmadığını gösterir. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Çizim alanı boyutunun onay işaretlerini ve eksen etiketlerini içerip içermediğini gösterir. False, boyutun çizim alanının boyutunu, onay işaretlerini ve eksen etiketlerini belirleyeceğini belirtir. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Çerçevenin gölgesi varsa doğrudur. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | [`ShapeProperties`](../chartframe/shapeproperties) nesne. |
| override [Width](../../aspose.cells.charts/chartarea/width) { get; set; } | Sağ alt köşe sütunundan yatay ofseti alır veya ayarlar. |
| override [X](../../aspose.cells.charts/chartarea/x) { get; set; } | Sol üst köşe sütunundan yatay ofseti alır veya alır. |
| override [Y](../../aspose.cells.charts/chartarea/y) { get; set; } | Sol üst köşe satırından dikey ofseti alır veya alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Çerçevenin konumunu otomatik olarak ayarlayın |

### Örnekler

```csharp

[C#]

//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();

//İlk çalışma sayfasının referansının alınması
Worksheet worksheet = workbook.Worksheets[0];

//"A1" hücresine örnek değer ekleme
worksheet.Cells["A1"].PutValue(50);

//"A2" hücresine örnek değer ekleme
worksheet.Cells["A2"].PutValue(100);

//"A3" hücresine örnek değer ekleme
worksheet.Cells["A3"].PutValue(150);

//"B1" hücresine örnek değer ekleme
worksheet.Cells["B1"].PutValue(60);

//"B2" hücresine örnek değer ekleme
worksheet.Cells["B2"].PutValue(32);

//"B3" hücresine örnek değer ekleme
worksheet.Cells["B3"].PutValue(50);

//Çalışma sayfasına grafik ekleme
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);

//Yeni eklenen grafiğin örneğine erişim
Chart chart = worksheet.Charts[chartIndex];

//"A1" hücresinden "B3"e kadar olan grafiğe NSeries (grafik veri kaynağı) ekleme
chart.NSeries.Add("A1:B3", true);

//Grafik Alanının Alınması
ChartArea chartArea = chart.ChartArea;

//Grafik alanının ön plan rengini ayarlama
chartArea.Area.ForegroundColor = Color.Yellow;

//Grafik Alanı Gölgesini Ayarlama
chartArea.Shadow = true;

//Excel dosyasını kaydetme
workbook.Save("book1.xls");

[VB.NET]

'Bir Çalışma Kitabı nesnesini başlatma
Dim workbook As Workbook = New Workbook()

'İlk çalışma sayfasının referansının alınması
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)

'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)

'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)

'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)

'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)

'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)

'Çalışma sayfasına grafik ekleme
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)

'Yeni eklenen grafiğin örneğine erişme
Dim chart As Chart = worksheet.Charts(chartIndex)

'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)

'Grafik Alanı Alma
Dim chartArea As ChartArea = chart.ChartArea

'Grafik alanının ön plan rengini ayarlama
chartArea.Area.ForegroundColor = Color.Yellow

'Grafik Alanı Gölgesini Ayarlama
chartArea.Shadow = True

'Excel dosyasını kaydetme
workbook.Save("book1.xls")
```

### Ayrıca bakınız

* class [ChartFrame](../chartframe)
* ad alanı [Aspose.Cells.Charts](../../aspose.cells.charts)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

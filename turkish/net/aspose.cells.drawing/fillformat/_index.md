---
title: FillFormat
second_title: Aspose.Cells for .NET API Referansı
description: Bir şekil için dolgu biçimlendirmesini temsil eden nesneyi kapsüller.
type: docs
weight: 1970
url: /tr/net/aspose.cells.drawing/fillformat/
---
## FillFormat class

Bir şekil için dolgu biçimlendirmesini temsil eden nesneyi kapsüller.

```csharp
public class FillFormat
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | Doldurma türünü alır ve ayarlar |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | Belirtilen dolgu için degrade rengi 1'i döndürür. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | Belirtilen dolgu için 2 degrade rengini döndürür. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | Belirtilen dolgu için degrade renk türünü döndürür. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | Belirtilen dolgu için degrade derecesini verir. Yalnızca Excel 2007 için geçerlidir. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | Alır[`GradientFill`](./gradientfill) nesne. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | Belirtilen dolgu için degrade stilini döndürür. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | Belirtilen dolgu için degrade varyantını döndürür. Yalnızca Excel 2007 için geçerlidir. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | Resim görüntü verilerini alır ve ayarlar. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | Bir alanın görüntüleme düzenini temsil eder. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | Alır[`PatternFill`](./patternfill) nesne. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | Resim biçimi türünü alır ve ayarlar. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | Belirtilen dolgu için degrade ön ayar rengini döndürür. |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | Resim biçimi ölçeğini alır ve ayarlar. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | Alır[`SolidFill`](./solidfill) nesne. |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | Belirtilen dolgu için doku türünü temsil eder. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | Alır[`TextureFill`](./texturefill) nesne. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | Alanın şeffaflık derecesini 0.0 (opak) ile 1.0 (net) arasında bir değer olarak döndürür veya ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode)() | Karma kodunu alır. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | Belirtilen dolguyu tek renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | Belirtilen dolguyu önceden ayarlanmış renk gradyanına ayarlar. Yalnızca Excel 2007 için geçerlidir. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Belirtilen dolguyu iki renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Belirtilen dolguyu iki renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir. |

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
int seriesIndex = chart.NSeries.Add("A1:B4", true);
// NSeries'in kategori verileri için veri kaynağının ayarlanması
chart.NSeries.CategoryData = "C1:C4";
// 2. NSeries alanını bir degradeyle doldurma
chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1);

[Visual Basic]

Bir Çalışma Kitabı nesnesini başlatma
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
Dim seriesIndex As Int32 = chart.NSeries.Add("A1:B4", True)
'NSeries kategori verileri için veri kaynağını ayarlama
chart.NSeries.CategoryData = "C1:C4"
'2. NSeries alanını bir degradeyle doldurma
chart.NSeries(seriesIndex).Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1)
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

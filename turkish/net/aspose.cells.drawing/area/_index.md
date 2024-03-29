---
title: Area
second_title: Aspose.Cells for .NET API Referansı
description: Bir alan biçimini temsil eden nesneyi kapsüller.
type: docs
weight: 1760
url: /tr/net/aspose.cells.drawing/area/
---
## Area class

Bir alan biçimini temsil eden nesneyi kapsüller.

```csharp
public class Area
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor) { get; set; } | Arka planı alır veya ayarlarColor arasında[`Area`](../area) . |
| [FillFormat](../../aspose.cells.drawing/area/fillformat) { get; } | Bir belirtilen grafik veya şekil için dolgu biçimlendirme özelliklerini içeren nesne. |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor) { get; set; } | Ön planı alır veya ayarlarColor . |
| [Formatting](../../aspose.cells.drawing/area/formatting) { get; set; } | Alanın biçimlendirmesini temsil eder. |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative) { get; set; } | Özellik doğruysa ve grafik noktasının değeri negatif bir sayıysa, ön plan rengi ve arka plan rengi değiştirilir. |
| [Transparency](../../aspose.cells.drawing/area/transparency) { get; set; } | Alanın şeffaflık derecesini 0.0 (opak) ile 1.0 (net) arasında bir değer olarak döndürür veya ayarlar. |

### Örnekler

```csharp

[C#]
//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();
//Workbook nesnesine yeni bir çalışma sayfası ekleme
int sheetIndex = workbook.Worksheets.Add();
//Yeni eklenen çalışma sayfasının sayfa indeksini geçerek referansının alınması
Worksheet worksheet = workbook.Worksheets[sheetIndex];
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
//Plot alanının ön plan rengini ayarlama
chart.PlotArea.Area.ForegroundColor = Color.Blue;
//Grafik alanının ön plan rengini ayarlama
chart.ChartArea.Area.ForegroundColor = Color.Yellow;
// 1. NSeries alanının ön plan rengini ayarlama
chart.NSeries[0].Area.ForegroundColor = Color.Red;
// 1. NSeries noktasının alanının ön plan rengini ayarlama
chart.NSeries[0].Points[0].Area.ForegroundColor = Color.Cyan;
//Excel dosyasını kaydetme
workbook.Save("book1.xls");

[Visual Basic]

'Bir Çalışma Kitabı nesnesini başlatma
Dim workbook As Workbook = New Workbook()
'Çalışma Kitabı nesnesine yeni bir çalışma sayfası ekleme
Dim sheetIndex As Integer = workbook.Worksheets.Add()
'Yeni eklenen çalışma sayfasının sayfa indeksini geçerek referansını alma
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
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
'Çizim alanının ön plan rengini ayarlama
chart.PlotArea.Area.ForegroundColor = Color.Blue
'Grafik alanının ön plan rengini ayarlama
chart.ChartArea.Area.ForegroundColor = Color.Yellow
'1. NSeries alanının ön plan rengini ayarlama
chart.NSeries(0).Area.ForegroundColor = Color.Red
'1. NSeries noktasının alanının ön plan rengini ayarlama
chart.NSeries(0).Points(0).Area.ForegroundColor = Color.Cyan
'Excel dosyasını kaydetme
workbook.Save("book1.xls")
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

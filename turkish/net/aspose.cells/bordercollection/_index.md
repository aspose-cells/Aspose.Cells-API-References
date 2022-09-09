---
title: BorderCollection
second_title: Aspose.Cells for .NET API Referansı
description: Bir koleksiyonu kapsüllerBorder./border nesneler.
type: docs
weight: 150
url: /tr/net/aspose.cells/bordercollection/
---
## BorderCollection class

Bir koleksiyonu kapsüller[`Border`](../border) nesneler.

```csharp
public class BorderCollection
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [DiagonalColor](../../aspose.cells/bordercollection/diagonalcolor) { get; set; } | Alır veya ayarlarColor çapraz çizgiler. |
| [DiagonalStyle](../../aspose.cells/bordercollection/diagonalstyle) { get; set; } | Çapraz çizgilerin stilini alır veya ayarlar. |
| [Item](../../aspose.cells/bordercollection/item) { get; } | [`Border`](../border) belirtilen dizindeki öğe. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [SetColor](../../aspose.cells/bordercollection/setcolor)(Color) | Color koleksiyondaki tüm kenarlıklar. |
| [SetStyle](../../aspose.cells/bordercollection/setstyle)(CellBorderType) | Koleksiyonun tüm kenarlıklarının stilini ayarlar. |

### Örnekler

```csharp

[C#]

//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();

//Excel nesnesine yeni bir çalışma sayfası ekleme
workbook.Worksheets.Add();

//Yeni eklenen çalışma sayfasının sayfa indeksini geçerek referansının alınması
Worksheet worksheet = workbook.Worksheets[0];

//Çalışma sayfasından "A1" hücresine erişim
Cell cell = worksheet.Cells["A1"];

//"A1" hücresine değer ekleme
cell.PutValue("Visit Aspose!");

Style style = cell.GetStyle();

//Üst sınırın çizgi stilini ayarlama
style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;

//Üst sınırın rengini ayarlama
style.Borders[BorderType.TopBorder].Color = Color.Black;

//Alt sınırın çizgi stilini ayarlama
style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thick;

//Alt sınırın rengini ayarlama
style.Borders[BorderType.BottomBorder].Color = Color.Black;

//Sol kenarlığın çizgi stilini ayarlama
style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thick;

//Sol kenarlığın rengini ayarlama
style.Borders[BorderType.LeftBorder].Color = Color.Black;

//Sağ sınırın çizgi stilini ayarlama
style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thick;

//Sağ kenarlığın rengini ayarlama
style.Borders[BorderType.RightBorder].Color = Color.Black;

cell.SetStyle(style);

//Excel dosyasını kaydetme
workbook.Save("book1.xls");

[VB.NET]

'Bir Çalışma Kitabı nesnesini başlatma
Dim workbook As Workbook = New Workbook()

'Çalışma Kitabı nesnesine yeni bir çalışma sayfası ekleme
workbook.Worksheets.Add()

'Yeni eklenen çalışma sayfasının sayfa indeksini geçerek referansını alma
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Accessing the "A1" cell from the worksheet
Dim cell As Cell = worksheet.Cells("A1")

'Adding some value to the "A1" cell
cell.PutValue("Visit Aspose!")

Dim style as Style = cell.GetStyle()

'Üst sınırın çizgi stilini ayarlama
style.Borders(BorderType.TopBorder).LineStyle = CellBorderType.Thick

'Üst sınırın rengini ayarlama
style.Borders(BorderType.TopBorder).Color = Color.Black

'Alt sınırın çizgi stilini ayarlama
style.Borders(BorderType.BottomBorder).LineStyle = CellBorderType.Thick

'Alt kenarlığın rengini ayarlama
style.Borders(BorderType.BottomBorder).Color = Color.Black

'Sol kenarlığın çizgi stilini ayarlama
style.Borders(BorderType.LeftBorder).LineStyle = CellBorderType.Thick

'Sol kenarlığın rengini ayarlama
style.Borders(BorderType.LeftBorder).Color = Color.Black

'Sağ kenarlığın çizgi stilini ayarlama
style.Borders(BorderType.RightBorder).LineStyle = CellBorderType.Thick

'Sağ kenarlığın rengini ayarlama
style.Borders(BorderType.RightBorder).Color = Color.Black

cell.SetStyle(style)

'Excel dosyasını kaydetme
workbook.Save("book1.xls")
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
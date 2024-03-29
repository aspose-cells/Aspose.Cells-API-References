---
title: Font
second_title: Aspose.Cells for .NET API Referansı
description: Bir elektronik tabloda kullanılan yazı tipi nesnesini kapsüller.
type: docs
weight: 3490
url: /tr/net/aspose.cells/font/
---
## Font class

Bir elektronik tabloda kullanılan yazı tipi nesnesini kapsüller.

```csharp
public class Font
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor) { get; set; } | 32 bit ARGB değeriyle rengi alır ve ayarlar. |
| [CapsType](../../aspose.cells/font/capstype) { get; set; } | Metin büyük harf türünü alır ve ayarlar. |
| [Charset](../../aspose.cells/font/charset) { get; set; } | Karakter setini temsil eder. |
| [Color](../../aspose.cells/font/color) { get; set; } | Alır veya ayarlarColor yazı tipinin. |
| [DoubleSize](../../aspose.cells/font/doublesize) { get; set; } | Yazı tipinin çift boyutunu alır ve ayarlar. |
| [IsBold](../../aspose.cells/font/isbold) { get; set; } | Yazı tipinin kalın olup olmadığını belirten bir değer alır veya ayarlar. |
| [IsItalic](../../aspose.cells/font/isitalic) { get; set; } | Yazı tipinin italik olup olmadığını belirten bir değer alır veya ayarlar. |
| [IsNormalizeHeights](../../aspose.cells/font/isnormalizeheights) { get; set; } | Metnin çalıştırılmasına uygulanacak yüksekliğin normalleştirilmesinin olup olmadığını gösterir. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout) { get; set; } | Yazı tipinin tek üstü çizili olup olmadığını belirten bir değer alır veya ayarlar. |
| [IsSubscript](../../aspose.cells/font/issubscript) { get; set; } | Yazı tipinin alt simge olup olmadığını gösteren bir değer alır veya ayarlar. |
| [IsSuperscript](../../aspose.cells/font/issuperscript) { get; set; } | Yazı tipinin süper komut dosyası olup olmadığını belirten bir değer alır veya ayarlar. |
| virtual [Name](../../aspose.cells/font/name) { get; set; } | Dosyanın adını alır veya ayarlar.[`Font`](../font) . |
| [SchemeType](../../aspose.cells/font/schemetype) { get; set; } | Yazı tipinin şema türünü alır ve ayarlar. |
| [ScriptOffset](../../aspose.cells/font/scriptoffset) { get; set; } | Yüzde biriminde komut dosyası ofsetini alır ve ayarlar |
| [Size](../../aspose.cells/font/size) { get; set; } | Yazı tipinin boyutunu alır veya ayarlar. |
| [StrikeType](../../aspose.cells/font/striketype) { get; set; } | Metnin vuruş türünü alır. |
| [ThemeColor](../../aspose.cells/font/themecolor) { get; set; } | Tema rengini alır ve ayarlar. |
| [Underline](../../aspose.cells/font/underline) { get; set; } | Yazı tipi alt çizgi türünü alır veya ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Equals](../../aspose.cells/font/equals#equals)(Font) | İki yazı tipinin eşit olup olmadığını kontrol eder. |
| override [ToString](../../aspose.cells/font/tostring)() | Geçerli Cell nesnesini temsil eden bir dize döndürür. |

### Örnekler

```csharp

[C#]

//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();

//Yeni eklenen çalışma sayfasının sayfa indeksini geçerek referansının alınması
Worksheet worksheet = workbook.Worksheets[0];

//Çalışma sayfasından "A1" hücresine erişim
Aspose.Cells.Cell cell = worksheet.Cells["A1"];

//"A1" hücresine değer ekleme
cell.PutValue("Hello Aspose!");

Aspose.Cells.Font font = cell.GetStyle().Font;

//Yazı tipi adını "Times New Roman" olarak ayarlama
font.Name = "Times New Roman";

// Yazı tipi boyutunu 14 olarak ayarlama
font.Size = 14;

// yazı tipi rengini Kırmızı olarak ayarlama
font.Color = System.Drawing.Color.Red;           

//Excel dosyasını kaydetme
workbook.Save(@"dest.xls");

[VB.NET]

'Bir Çalışma Kitabı nesnesini başlatma
Dim workbook As Workbook = New Workbook()

'Yeni eklenen çalışma sayfasının sayfa indeksini geçerek referansını alma
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Accessing the "A1" cell from the worksheet
Dim cell As Aspose.Cells.Cell = worksheet.Cells("A1")

'Adding some value to the "A1" cell
cell.PutValue("Hello Aspose!")

Dim font As Aspose.Cells.Font = cell.GetStyle().Font

'Setting the font name to "Times New Roman"
font.Name = "Times New Roman"

'Yazı tipi boyutunu 14 olarak ayarlama
font.Size = 14

'yazı tipi rengini Kırmızı olarak ayarlama
font.Color = System.Drawing.Color.Red

'Excel dosyasını kaydetme
workbook.Save("dest.xls")
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

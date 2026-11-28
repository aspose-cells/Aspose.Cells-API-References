---
title: "Class TextBoxOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Texts.TextBoxOptions class. Şeklin metin seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textboxoptions/
---
## TextBoxOptions class

Şeklin metin seçeneklerinin temsilidir

```csharp
public class TextBoxOptions
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AllowTextToOverflow](../../aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/) { get; set; } | Metnin şekli taşmasına izin verilip verilmeyeceği. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/textboxoptions/bottommarginpt/) { get; set; } | Alt kenar boşluğunu Point biriminde döndürür |
| [LeftMarginPt](../../aspose.cells.drawing.texts/textboxoptions/leftmarginpt/) { get; set; } | Sol kenar boşluğunu Nokta biriminde alır ve ayarlar. |
| [ResizeToFitText](../../aspose.cells.drawing.texts/textboxoptions/resizetofittext/) { get; set; } | Şekli metne sığdırmak için yeniden boyutlandırıp boyutlandırmayacağını gösterir |
| [RightMarginPt](../../aspose.cells.drawing.texts/textboxoptions/rightmarginpt/) { get; set; } | Sağ kenar boşluğunu Nokta biriminde alır ve ayarlar. |
| [ShapeTextDirection](../../aspose.cells.drawing.texts/textboxoptions/shapetextdirection/) { get; set; } | Belirli bir metin gövdesi içinde metin görüntüleme yönünü alır veya ayarlar. Excel'de "Format Shape - Text Options - Text Box - Text direction" ile eşdeğerdir |
| [ShapeTextVerticalAlignment](../../aspose.cells.drawing.texts/textboxoptions/shapetextverticalalignment/) { get; set; } | Excel'de "Format Shape - Text Options - Text Box - Vertical Alignment" ile eşleşir. |
| [TopMarginPt](../../aspose.cells.drawing.texts/textboxoptions/topmarginpt/) { get; set; } | Üst kenar boşluğunu Nokta biriminde alır ve ayarlar. |
| [WrapTextInShape](../../aspose.cells.drawing.texts/textboxoptions/wraptextinshape/) { get; set; } | Şekil içinde metin kaydırmayı belirtir. False - Metin gövdesinde kaydırma olmaz. True - Metin gövdesinde kaydırma olur. |

### Örnekler

```csharp

[C#]
//Workbook nesnesi örnekleniyor
Workbook workbook = new Workbook();
int index = workbook.Worksheets[0].TextBoxes.Add(0, 0, 350, 350);
Shape shape = workbook.Worksheets[0].TextBoxes[index];
shape.Text = "This is test.";

//işinizi yapın

//Excel dosyasını kaydet.
workbook.Save("exmaple.xlsx");
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)



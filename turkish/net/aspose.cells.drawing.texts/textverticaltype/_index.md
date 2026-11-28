---
title: "Enum TextVerticalType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Texts.TextVerticalType enum. Metnin yön tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textverticaltype/
---
## TextVerticalType enumeration

Metin doğrudan türünü temsil eder.

```csharp
public enum TextVerticalType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Vertical | `0` | Doğu Asya Dikey görüntüleme. |
| Horizontal | `1` | Yatay metin. |
| VerticalLeftToRight | `2` | Dikey olarak görüntülenir ve metin yukarıdan aşağıya, ardından SOL'dan SAĞ'a akar |
| Vertical90 | `3` | Her satır saat yönünde 90 derece döndürülür |
| Vertical270 | `4` | Her satır saat yönünde 270 derece döndürülür |
| Stacked | `5` | Metnin tamamının dikey olup olmadığını belirler |
| StackedRightToLeft | `6` | Dikey WordArt'ın soldan sağa yerine sağdan sola gösterilmesi gerektiğini belirtir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextVerticalTypeDemo
    {
        public static void TextVerticalTypeExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir dikdörtgen şekli ekleme
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);

            // Şeklin metin hizalama ayarlarına erişme
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Metin dikey tipini Yatay olarak ayarlama
            shapeTextAlignment.TextVerticalType = TextVerticalType.Horizontal;

            // Demonstrasyon için diğer özellikleri ayarlama
            shapeTextAlignment.IsTextWrapped = true;
            shapeTextAlignment.RotateTextWithShape = true;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.RotationAngle = 90;
            shapeTextAlignment.IsLockedText = false;
            shapeTextAlignment.AutoSize = false;
            shapeTextAlignment.TextShapeType = AutoShapeType.TextBox;
            shapeTextAlignment.TopMarginPt = 2.0d;
            shapeTextAlignment.BottomMarginPt = 2.0d;
            shapeTextAlignment.LeftMarginPt = 2.0d;
            shapeTextAlignment.RightMarginPt = 2.0d;
            shapeTextAlignment.IsAutoMargin = true;
            shapeTextAlignment.NumberOfColumns = 1;

            // Çalışma kitabını kaydetme
            workbook.Save("TextVerticalTypeExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)



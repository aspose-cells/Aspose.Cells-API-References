---
title: "Sınıf ShapeTextAlignment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Texts.ShapeTextAlignment sınıfı. Şekillerin metin hizalama ayarını temsil eder."
type: docs
url: /tr/net/aspose.cells.drawing.texts/shapetextalignment/
---
## ShapeTextAlignment class

Şeklin metin hizalamasının ayarının temsilidir;

```csharp
public class ShapeTextAlignment
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AutoSize](../../aspose.cells.drawing.texts/shapetextalignment/autosize/) { get; set; } | Şeklin boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/bottommarginpt/) { get; set; } | Alt kenar boşluğunu Point biriminde döndürür |
| [IsAutoMargin](../../aspose.cells.drawing.texts/shapetextalignment/isautomargin/) { get; set; } | Metin çerçevesinin kenar boşluğunun otomatik olup olmadığını gösterir. |
| [IsLockedText](../../aspose.cells.drawing.texts/shapetextalignment/islockedtext/) { get; set; } | Çalışma sayfası korunduğunda şeklin kilitli olup olmadığını gösterir. |
| [IsTextWrapped](../../aspose.cells.drawing.texts/shapetextalignment/istextwrapped/) { get; set; } | Metin içeren şeklin metin sarma türünü alır veya ayarlar. |
| [LeftMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/leftmarginpt/) { get; set; } | Sol kenar boşluğunu Point biriminde döndürür |
| [NumberOfColumns](../../aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/) { get; set; } | Sınırlayıcı dikdörtgendeki metin sütun sayısını alır ve ayarlar. |
| [RightMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/rightmarginpt/) { get; set; } | Sağ kenar boşluğunu Point biriminde döndürür |
| [RotateTextWithShape](../../aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape/) { get; set; } | Şekilde metin döndürülüp döndürülmediğini gösterir. |
| [RotationAngle](../../aspose.cells.drawing.texts/shapetextalignment/rotationangle/) { get; set; } | Şeklin dönüşünü alır ve ayarlar. |
| [TextHorizontalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow/) { get; set; } | Metin kutusunun metin yatay taşma türünü alır ve ayarlar. |
| [TextShapeType](../../aspose.cells.drawing.texts/shapetextalignment/textshapetype/) { get; set; } | Metnin dönüşüm türünü alır ve ayarlar. |
| [TextVerticalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow/) { get; set; } | Metin kutusunun metin dikey taşma türünü alır ve ayarlar. |
| [TextVerticalType](../../aspose.cells.drawing.texts/shapetextalignment/textverticaltype/) { get; set; } | Metin yönünü alır ve ayarlar. |
| [TopMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/topmarginpt/) { get; set; } | Üst kenar boşluğunu Point biriminde döndürür |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.cells.drawing.texts/shapetextalignment/equals/)(object) | Bu örneğin, belirtilen başka bir `ShapeTextAlignment` nesnesiyle aynı değere sahip olup olmadığını belirler. |
| override [GetHashCode](../../aspose.cells.drawing.texts/shapetextalignment/gethashcode/)() |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class ShapeTextAlignmentDemo
    {
        public static void ShapeTextAlignmentExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir dikdörtgen şekli ekleme
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);

            // ShapeTextAlignment nesnesine erişim
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Özellikleri ayarlama
            shapeTextAlignment.IsTextWrapped = true;
            shapeTextAlignment.RotateTextWithShape = true;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.RotationAngle = 90;
            shapeTextAlignment.TextVerticalType = TextVerticalType.Horizontal;
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
            workbook.Save("ShapeTextAlignmentExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)



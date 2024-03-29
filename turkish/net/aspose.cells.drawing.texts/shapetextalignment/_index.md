---
title: ShapeTextAlignment
second_title: Aspose.Cells for .NET API Referansı
description: Şeklin metin hizalama ayarını temsil eder
type: docs
weight: 2940
url: /tr/net/aspose.cells.drawing.texts/shapetextalignment/
---
## ShapeTextAlignment class

Şeklin metin hizalama ayarını temsil eder;

```csharp
public class ShapeTextAlignment
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AutoSize](../../aspose.cells.drawing.texts/shapetextalignment/autosize) { get; set; } | Şeklin boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/bottommarginpt) { get; set; } | Alt kenar boşluğunu Points biriminde döndürür |
| [IsAutoMargin](../../aspose.cells.drawing.texts/shapetextalignment/isautomargin) { get; set; } | Metin çerçevesinin kenar boşluğunun otomatik olup olmadığını gösterir. |
| [IsTextWrapped](../../aspose.cells.drawing.texts/shapetextalignment/istextwrapped) { get; set; } | Metni içeren şeklin metin sarmalı türünü alır ve ayarlar. |
| [LeftMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/leftmarginpt) { get; set; } | Sol kenar boşluğunu Points biriminde döndürür |
| [RightMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/rightmarginpt) { get; set; } | Sağ kenar boşluğunu Points biriminde döndürür |
| [RotateTextWithShape](../../aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape) { get; set; } | Metnin şekil ile döndürülüp döndürülmediğini gösterir. |
| [RotationAngle](../../aspose.cells.drawing.texts/shapetextalignment/rotationangle) { get; set; } | Şeklin dönüşünü alır ve ayarlar. |
| [TextHorizontalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow) { get; set; } | Metin kutusunun metin yatay taşma türünü alır ve ayarlar. |
| [TextShapeType](../../aspose.cells.drawing.texts/shapetextalignment/textshapetype) { get; set; } | Metnin dönüştürme türünü alır ve ayarlar. |
| [TextVerticalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow) { get; set; } | Metin kutusunun metin dikey taşma türünü alır ve ayarlar. |
| [TextVerticalType](../../aspose.cells.drawing.texts/shapetextalignment/textverticaltype) { get; set; } | Metin yönünü alır ve ayarlar. |
| [TopMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/topmarginpt) { get; set; } | Points biriminde üst kenar boşluğunu döndürür |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [Equals](../../aspose.cells.drawing.texts/shapetextalignment/equals)(object) | Bu örneğin belirtilen başka bir örnekle aynı değere sahip olup olmadığını belirler[`ShapeTextAlignment`](../shapetextalignment) nesne. |
| override [GetHashCode](../../aspose.cells.drawing.texts/shapetextalignment/gethashcode)() |  |

### Örnekler

```csharp

[C#]
//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();
Shape shape = workbook.Worksheets[0].Shapes.AddRectangle(1, 0, 1, 0, 50, 100);
Aspose.Cells.Drawing.Texts.ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

//işini yap

```

### Ayrıca bakınız

* ad alanı [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

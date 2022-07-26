---
title: LineFormat
second_title: Aspose.Cells for .NET API Referansı
description: Satırın tüm ayarlarını temsil eder.
type: docs
weight: 2220
url: /tr/net/aspose.cells.drawing/lineformat/
---
## LineFormat class

Satırın tüm ayarlarını temsil eder.

```csharp
public class LineFormat : FillFormat
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [BeginArrowheadLength](../../aspose.cells.drawing/lineformat/beginarrowheadlength) { get; set; } | Çizginin başlangıç ok uzunluğu türünü alır ve ayarlar. |
| [BeginArrowheadStyle](../../aspose.cells.drawing/lineformat/beginarrowheadstyle) { get; set; } | Çizginin başlangıç ok türünü alır ve ayarlar. |
| [BeginArrowheadWidth](../../aspose.cells.drawing/lineformat/beginarrowheadwidth) { get; set; } | Çizginin başlangıç ok genişliği türünü alır ve ayarlar. |
| [CapType](../../aspose.cells.drawing/lineformat/captype) { get; set; } | Bitiş büyük harflerini belirtir. |
| [CompoundType](../../aspose.cells.drawing/lineformat/compoundtype) { get; set; } | Satır bileşik türünü belirtir. |
| [DashStyle](../../aspose.cells.drawing/lineformat/dashstyle) { get; set; } | Çizgi tipini belirtir. |
| [EndArrowheadLength](../../aspose.cells.drawing/lineformat/endarrowheadlength) { get; set; } | Çizginin bitiş ok uzunluğu türünü alır ve ayarlar. |
| [EndArrowheadStyle](../../aspose.cells.drawing/lineformat/endarrowheadstyle) { get; set; } | Çizginin bitiş ok türünü alır ve ayarlar. |
| [EndArrowheadWidth](../../aspose.cells.drawing/lineformat/endarrowheadwidth) { get; set; } | Çizginin bitiş ok genişliği türünü alır ve ayarlar. |
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | Doldurma türünü alır ve ayarlar |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | Belirtilen dolgu için degrade rengi 1'i döndürür. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | Belirtilen dolgu için 2 degrade rengini döndürür. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | Belirtilen dolgu için degrade renk türünü döndürür. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | Belirtilen dolgu için degrade derecesini verir. Yalnızca Excel 2007 için geçerlidir. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | Alır[`GradientFill`](../fillformat/gradientfill) nesne. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | Belirtilen dolgu için degrade stilini döndürür. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | Belirtilen dolgu için degrade varyantını döndürür. Yalnızca Excel 2007 için geçerlidir. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | Resim görüntü verilerini alır ve ayarlar. |
| [JoinType](../../aspose.cells.drawing/lineformat/jointype) { get; set; } | Satır birleştirme türünü belirtir. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | Bir alanın görüntüleme düzenini temsil eder. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | Alır[`PatternFill`](../fillformat/patternfill) nesne. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | Resim biçimi türünü alır ve ayarlar. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | Belirtilen dolgu için degrade ön ayar rengini döndürür. |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | Resim biçimi ölçeğini alır ve ayarlar. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | Alır[`SolidFill`](../fillformat/solidfill) nesne. |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | Belirtilen dolgu için doku türünü temsil eder. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | Alır[`TextureFill`](../fillformat/texturefill) nesne. |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | Alanın şeffaflık derecesini 0.0 (opak) ile 1.0 (net) arasında bir değer olarak döndürür veya ayarlar. |
| [Weight](../../aspose.cells.drawing/lineformat/weight) { get; set; } | Çizginin ağırlığını puan birimi cinsinden alır veya ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/lineformat/equals)(object) | Bu örneğin belirtilen başka bir örnekle aynı değere sahip olup olmadığını belirler[`LineFormat`](../lineformat) nesne. |
| override [GetHashCode](../../aspose.cells.drawing/lineformat/gethashcode)() | Karma kodunu alır. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | Belirtilen dolguyu tek renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | Belirtilen dolguyu önceden ayarlanmış renk gradyanına ayarlar. Yalnızca Excel 2007 için geçerlidir. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient)(Color, Color, GradientStyleType, int) | Belirtilen dolguyu iki renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Belirtilen dolguyu iki renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir. |

### Örnekler

```csharp

[C#]
//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();
ShapeCollection shapes = workbook.Worksheets[0].Shapes;
Shape shape = shapes.AddRectangle(1, 0, 1, 0, 50, 100);
LineFormat lineFmt = shape.Line;

//işini yap

```

### Ayrıca bakınız

* class [FillFormat](../fillformat)
* ad alanı [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->

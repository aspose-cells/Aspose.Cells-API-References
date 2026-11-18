---
title: "ShapePath Sınıfı"
linktitle: "ShapePath"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "ShapePath sınıfı. Go'da shapepath'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/shapepath/
---

## ShapePath class

Bir dizi hareket, çizgi ve eğriden oluşan ve birleştirildiğinde geometrik bir şekil oluşturacak bir oluşturma yolunu temsil eder.

```go

type ShapePath struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewShapePath](./newshapepath/) | ShapePath sınıfının yeni bir örneğini başlatır. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetPathSegments](./getpathsegments/) | ShapeSegmentPathCollection listesini alır |
| [GetWidthPixel](./getwidthpixel/) | Bu yolun genişliğini piksel biriminde alır. |
| [SetWidthPixel](./setwidthpixel/) | Bu yolun genişliğini piksel biriminde alır. |
| [GetHeightPixel](./getheightpixel/) | Bu yolun yüksekliğini piksel biriminde alır. |
| [SetHeightPixel](./setheightpixel/) | Bu yolun yüksekliğini piksel biriminde alır. |
| [MoveTo](./moveto/) | Belirtilen noktadan mevcut şekli kapatmadan yeni bir şekil başlatır. Yola eklenen sonraki tüm noktalar bu yeni şekle eklenir. Birim: Piksel. |
| [LineTo](./lineto/) | Mevcut şekle bir çizgi segmenti ekler. Başlangıç noktası mevcut şeklin bitiş noktasıdır. Birim: Piksel. |
| [CubicBezierTo](./cubicbezierto/) | Mevcut şekle kübik Bézier eğrisi ekler. Başlangıç noktası mevcut şeklin bitiş noktasıdır. Birim: Piksel. |
| [ArcTo](./arcto/) | Mevcut şekle eliptik bir yay ekler. Başlangıç noktası mevcut şeklin bitiş noktasıdır. |
| [Close](./close/) | Mevcut şekli kapatır ve yeni bir şekil başlatır. Eğer mevcut şekil bağlı çizgiler ve eğrilerden oluşan bir dizi içeriyorsa, yöntem son noktayı başlangıç noktasına bir çizgiyle bağlayarak döngüyü kapatır. |

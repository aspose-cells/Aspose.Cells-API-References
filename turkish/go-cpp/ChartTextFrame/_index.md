---
title: "ChartTextFrame Sınıfı"
linktitle: "ChartTextFrame"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "ChartTextFrame sınıfı. Go'da charttextframe nesnesini temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/charttextframe/
---

## ChartTextFrame class

Metin içeren çerçeve nesnesini temsil eden nesneyi kapsüller.

```go

type ChartTextFrame struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewChartTextFrame](./newcharttextframe/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [IsDeleted](./isdeleted/) | Bu veri etiketinin silinip silinmediğini gösterir. |
| [SetIsDeleted](./setisdeleted/) | Bu veri etiketinin silinip silinmediğini gösterir. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Metnin yatay hizalamasını alır ve ayarlar. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | Metnin yatay hizalamasını alır ve ayarlar. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | Metnin dikey hizalamasını alır veya ayarlar. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | Metnin dikey hizalamasını alır veya ayarlar. |
| [GetRotationAngle](./getrotationangle/) | Metin döndürme açısını temsil eder. |
| [SetRotationAngle](./setrotationangle/) | Metin döndürme açısını temsil eder. |
| [IsAutomaticRotation](./isautomaticrotation/) | Grafiğin metninin otomatik olarak döndürülüp döndürülmediğini gösterir. |
| [Characters](./characters/) | Metin içinde bir karakter aralığını temsil eden bir Characters nesnesi döndürür. |
| [GetReadingOrder](./getreadingorder/) | Metin okuma sırasını temsil eder. |
| [SetReadingOrder](./setreadingorder/) | Metin okuma sırasını temsil eder. |
| [IsResizeShapeToFitText](./isresizeshapetofittext/) | Bir şeklin içindeki metni tam olarak içerecek şekilde otomatik olarak sığdırılıp sığdırılmayacağını alır veya ayarlar. Otomatik sığdırma, bir şeklin içindeki metnin tamamını içerecek şekilde ölçeklendirilmesidir. |
| [SetIsResizeShapeToFitText](./setisresizeshapetofittext/) | Bir şeklin içindeki metni tam olarak içerecek şekilde otomatik olarak sığdırılıp sığdırılmayacağını alır veya ayarlar. Otomatik sığdırma, bir şeklin içindeki metnin tamamını içerecek şekilde ölçeklendirilmesidir. |
| [IsAutoText](./isautotext/) | Metnin otomatik olarak oluşturulduğunu gösterir. |
| [SetIsAutoText](./setisautotext/) | Metnin otomatik olarak oluşturulduğunu gösterir. |
| [GetText](./gettext/) | Çerçevenin başlığının metnini alır veya ayarlar. |
| [SetText](./settext/) | Çerçevenin başlığının metnini alır veya ayarlar. |
| [GetLinkedSource](./getlinkedsource/) | Çalışma sayfasına bir referansı alır ve ayarlar. |
| [SetLinkedSource](./setlinkedsource/) | Çalışma sayfasına bir referansı alır ve ayarlar. |
| [GetDirectionType](./getdirectiontype/) | Metnin yönünü alır veya ayarlar. |
| [SetDirectionType](./setdirectiontype/) | Metnin yönünü alır veya ayarlar. |
| [IsTextWrapped](./istextwrapped/) | Metnin kaydırılıp kaydırılmadığını gösteren bir değeri alır veya ayarlar. |
| [SetIsTextWrapped](./setistextwrapped/) | Metnin kaydırılıp kaydırılmadığını gösteren bir değeri alır veya ayarlar. |
| [IsInnerMode](./isinnermode/) | Çizim alanı boyutunun tık işaretlerini ve eksen etiketlerini içerip içermediğini gösterir.False, boyutun çizim alanını, tık işaretlerini ve eksen etiketlerini belirleyeceğini belirtir. |
| [SetIsInnerMode](./setisinnermode/) | Çizim alanı boyutunun tık işaretlerini ve eksen etiketlerini içerip içermediğini gösterir.False, boyutun çizim alanını, tık işaretlerini ve eksen etiketlerini belirleyeceğini belirtir. |
| [GetShadow](./getshadow/) | Çerçeve bir gölgeye sahipse True. |
| [SetShadow](./setshadow/) | Çerçeve bir gölgeye sahipse True. |
| [GetShapeProperties](./getshapeproperties/) | ShapeProperties nesnesini alır. |
| [IsDefaultPosBeSet](./isdefaultposbeset/) | Varsayılan konumun (DefaultX, DefaultY, DefaultWidth ve DefaultHeight) ayarlanıp ayarlanmadığını gösterir. |
| [GetDefaultXRatioToChart](./getdefaultxratiotochart/) | Varsayılan konumun x'ini grafik alanının Kesir biriminde temsil eder. |
| [GetDefaultYRatioToChart](./getdefaultyratiotochart/) | Varsayılan konumun y'sini grafik alanının kesir biriminde temsil eder. |
| [GetDefaultWidthRatioToChart](./getdefaultwidthratiotochart/) | Varsayılan konumun genişliğini grafik alanının Kesir biriminde temsil eder. |
| [GetDefaultHeightRatioToChart](./getdefaultheightratiotochart/) | Varsayılan konumun yüksekliğini grafik alanının kesir biriminde temsil eder. |
| [GetBorder](./getborder/) | Satırı alır</see>. |
| [GetArea](./getarea/) | Alanı alır</see>. |
| [GetTextOptions](./gettextoptions/) | Metnin seçeneklerini alır ve ayarlar. |
| [GetFont](./getfont/) | Belirtilen ChartFrame nesnesinin Font nesnesini alır. |
| [GetAutoScaleFont](./getautoscalefont/) | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa True. Varsayılan değer True. |
| [SetAutoScaleFont](./setautoscalefont/) | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa True. Varsayılan değer True. |
| [IsAutomaticSize](./isautomaticsize/) | Grafik çerçevesinin otomatik boyutlandırılıp boyutlandırılmadığını gösterir. |
| [SetIsAutomaticSize](./setisautomaticsize/) | Grafik çerçevesinin otomatik boyutlandırılıp boyutlandırılmadığını gösterir. |
| [GetXRatioToChart](./getxratiotochart/) | Grafik alanının oran birimlerinde sol üst köşenin x koordinatını alır veya ayarlar. |
| [SetXRatioToChart](./setxratiotochart/) | Grafik alanının oran birimlerinde sol üst köşenin x koordinatını alır veya ayarlar. |
| [GetYRatioToChart](./getyratiotochart/) | Grafik alanının oran biriminde sol üst köşenin y koordinatını alır veya ayarlar. |
| [SetYRatioToChart](./setyratiotochart/) | Grafik alanının oran biriminde sol üst köşenin y koordinatını alır veya ayarlar. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | Grafik alanının oran biriminde çerçevenin genişliğini alır veya ayarlar. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | Grafik alanının oran biriminde çerçevenin genişliğini alır veya ayarlar. |
| [GetHeightRatioToChart](./getheightratiotochart/) | Grafik alanının oran biriminde çerçevenin yüksekliğini alır veya ayarlar. |
| [SetHeightRatioToChart](./setheightratiotochart/) | Grafik alanının oran biriminde çerçevenin yüksekliğini alır veya ayarlar. |
| [GetXPixel](./getxpixel/) | Üst sol köşenin x koordinatını Piksel biriminde alır veya ayarlar. |
| [SetXPixel](./setxpixel/) | Üst sol köşenin x koordinatını Piksel biriminde alır veya ayarlar. |
| [GetYPixel](./getypixel/) | Üst sol köşenin y koordinatını piksel biriminde alır veya ayarlar. |
| [SetYPixel](./setypixel/) | Üst sol köşenin y koordinatını piksel biriminde alır veya ayarlar. |
| [GetWidthPixel](./getwidthpixel/) | Çerçevenin genişliğini Piksel biriminde alır veya ayarlar. |
| [SetWidthPixel](./setwidthpixel/) | Çerçevenin genişliğini Piksel biriminde alır veya ayarlar. |
| [GetHeightPixel](./getheightpixel/) | Çerçevenin yüksekliğini piksel biriminde alır veya ayarlar. |
| [SetHeightPixel](./setheightpixel/) | Çerçevenin yüksekliğini piksel biriminde alır veya ayarlar. |
| [SetPositionAuto](./setpositionauto/) | Çerçevenin konumunu otomatik olarak ayarla |

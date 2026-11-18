---
title: "ChartArea Sınıfı"
linktitle: "ChartArea"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "ChartArea sınıfı. Go'da chartarea nesnesini temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/chartarea/
---

## ChartArea class

Çalışma sayfasındaki çizelge alanını temsil eden nesneyi kapsüller.

```go

type ChartArea struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewChartArea](./newchartarea/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetXRatioToChart](./getxratiotochart/) | Grafik alanının sol üst köşe sütunundan yatay ofseti alır veya ayarlar, grafik alanının oranı olarak. |
| [SetXRatioToChart](./setxratiotochart/) | Grafik alanının sol üst köşe sütunundan yatay ofseti alır veya ayarlar, grafik alanının oranı olarak. |
| [GetYRatioToChart](./getyratiotochart/) | Grafik alanının sol üst köşe satırından dikey ofseti alır veya alır, grafik alanının oranı biriminde. |
| [SetYRatioToChart](./setyratiotochart/) | Grafik alanının sol üst köşe satırından dikey ofseti alır veya alır, grafik alanının oranı biriminde. |
| [GetHeightRatioToChart](./getheightratiotochart/) | Grafik alanının sağ alt köşe satırından dikey ofseti alır veya ayarlar, grafik alanının oranı biriminde. |
| [SetHeightRatioToChart](./setheightratiotochart/) | Grafik alanının sağ alt köşe satırından dikey ofseti alır veya ayarlar, grafik alanının oranı biriminde. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | Grafik alanının sağ alt köşe sütunundan yatay ofseti alır veya ayarlar, grafik alanının oranı biriminde. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | Grafik alanının sağ alt köşe sütunundan yatay ofseti alır veya ayarlar, grafik alanının oranı biriminde. |
| [GetFont](./getfont/) | Belirtilen ChartArea nesnesinin bir Font nesnesini alır. |
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
| [GetAutoScaleFont](./getautoscalefont/) | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa True. Varsayılan değer True. |
| [SetAutoScaleFont](./setautoscalefont/) | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa True. Varsayılan değer True. |
| [IsAutomaticSize](./isautomaticsize/) | Grafik çerçevesinin otomatik boyutlandırılıp boyutlandırılmadığını gösterir. |
| [SetIsAutomaticSize](./setisautomaticsize/) | Grafik çerçevesinin otomatik boyutlandırılıp boyutlandırılmadığını gösterir. |
| [GetXPixel](./getxpixel/) | Üst sol köşenin x koordinatını Piksel biriminde alır veya ayarlar. |
| [SetXPixel](./setxpixel/) | Üst sol köşenin x koordinatını Piksel biriminde alır veya ayarlar. |
| [GetYPixel](./getypixel/) | Üst sol köşenin y koordinatını piksel biriminde alır veya ayarlar. |
| [SetYPixel](./setypixel/) | Üst sol köşenin y koordinatını piksel biriminde alır veya ayarlar. |
| [GetWidthPixel](./getwidthpixel/) | Çerçevenin genişliğini Piksel biriminde alır veya ayarlar. |
| [SetWidthPixel](./setwidthpixel/) | Çerçevenin genişliğini Piksel biriminde alır veya ayarlar. |
| [GetHeightPixel](./getheightpixel/) | Çerçevenin yüksekliğini piksel biriminde alır veya ayarlar. |
| [SetHeightPixel](./setheightpixel/) | Çerçevenin yüksekliğini piksel biriminde alır veya ayarlar. |
| [SetPositionAuto](./setpositionauto/) | Çerçevenin konumunu otomatik olarak ayarla |

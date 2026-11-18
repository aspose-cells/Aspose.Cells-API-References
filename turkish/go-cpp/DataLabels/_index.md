---
title: "DataLabels Sınıfı"
linktitle: "DataLabels"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "DataLabels sınıfı. Go'da datalabels'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/datalabels/
---

## DataLabels class

Belirtilen Seri için tüm DataLabel nesnelerinin bir koleksiyonunu kapsüller.

```go

type DataLabels struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewDataLabels](./newdatalabels/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetBorder](./getborder/) | Satırı alır</see>. |
| [GetArea](./getarea/) | Alanı alır</see>. |
| [IsAutoText](./isautotext/) | Metnin otomatik olarak oluşturulduğunu gösterir. |
| [SetIsAutoText](./setisautotext/) | Metnin otomatik olarak oluşturulduğunu gösterir. |
| [GetDirectionType](./getdirectiontype/) | Metnin yönünü alır veya ayarlar. |
| [SetDirectionType](./setdirectiontype/) | Metnin yönünü alır veya ayarlar. |
| [GetText](./gettext/) | Veri etiketinin metnini alır veya ayarlar. |
| [SetText](./settext/) | Veri etiketinin metnini alır veya ayarlar. |
| [IsTextWrapped](./istextwrapped/) | Metnin kaydırılıp kaydırılmadığını gösteren bir değeri alır veya ayarlar. |
| [SetIsTextWrapped](./setistextwrapped/) | Metnin kaydırılıp kaydırılmadığını gösteren bir değeri alır veya ayarlar. |
| [GetBackgroundMode](./getbackgroundmode/) | Arka planın görüntüleme modunu alır ve ayarlar |
| [SetBackgroundMode](./setbackgroundmode/) | Arka planın görüntüleme modunu alır ve ayarlar |
| [GetShowValue](./getshowvalue/) | Belirtilen bir grafiğin veri etiketi değerlerinin görüntülenme davranışını temsil eder. True değerleri gösterir. False gizler. |
| [SetShowValue](./setshowvalue/) | Belirtilen bir grafiğin veri etiketi değerlerinin görüntülenme davranışını temsil eder. True değerleri gösterir. False gizler. |
| [GetShowCellRange](./getshowcellrange/) | Hücre aralığının veri etiketi olarak gösterilip gösterilmeyeceğini belirtir. |
| [SetShowCellRange](./setshowcellrange/) | Hücre aralığının veri etiketi olarak gösterilip gösterilmeyeceğini belirtir. |
| [GetShowPercentage](./getshowpercentage/) | Belirtilen bir grafiğin veri etiketi yüzde değerinin görüntülenme davranışını temsil eder. True yüzde değerini gösterir. False gizler. |
| [SetShowPercentage](./setshowpercentage/) | Belirtilen bir grafiğin veri etiketi yüzde değerinin görüntülenme davranışını temsil eder. True yüzde değerini gösterir. False gizler. |
| [GetShowBubbleSize](./getshowbubblesize/) | Belirtilen bir grafiğin veri etiketi yüzde değerinin görüntülenme davranışını temsil eder. True yüzde değerini gösterir. False yüzde değerini gizler. |
| [SetShowBubbleSize](./setshowbubblesize/) | Belirtilen bir grafiğin veri etiketi yüzde değerinin görüntülenme davranışını temsil eder. True yüzde değerini gösterir. False yüzde değerini gizler. |
| [GetShowCategoryName](./getshowcategoryname/) | Belirtilen bir grafiğin veri etiketi kategori adının görüntülenme davranışını temsil eder. True grafikteki veri etiketleri için kategori adını gösterir. False gizler. |
| [SetShowCategoryName](./setshowcategoryname/) | Belirtilen bir grafiğin veri etiketi kategori adının görüntülenme davranışını temsil eder. True grafikteki veri etiketleri için kategori adını gösterir. False gizler. |
| [GetShowSeriesName](./getshowseriesname/) | Seri adının grafikteki veri etiketlerinde gösterilip gösterilmeyeceğini belirtir. True seri adını gösterir. False gizler. |
| [SetShowSeriesName](./setshowseriesname/) | Seri adının grafikteki veri etiketlerinde gösterilip gösterilmeyeceğini belirtir. True seri adını gösterir. False gizler. |
| [GetShowLegendKey](./getshowlegendkey/) | Belirtilen bir grafiğin veri etiketi lejand anahtarının görüntülenme davranışını temsil eder. True veri etiketi lejand anahtarı görünürse. |
| [SetShowLegendKey](./setshowlegendkey/) | Belirtilen bir grafiğin veri etiketi lejand anahtarının görüntülenme davranışını temsil eder. True veri etiketi lejand anahtarı görünürse. |
| [Get_NumberFormat](./get_numberformat/) | DataLabels nesnesi için biçim dizesini temsil eder. |
| [SetNumberFormat](./setnumberformat/) | DataLabels nesnesi için biçim dizesini temsil eder. |
| [GetNumber](./getnumber/) | Yerleşik sayı biçimini alır ve ayarlar. |
| [SetNumber](./setnumber/) | Yerleşik sayı biçimini alır ve ayarlar. |
| [GetNumberFormatLinked](./getnumberformatlinked/) | Sayı biçimi hücrelere bağlıysa (etiketlerdeki sayı biçimi hücrelerde değiştiğinde değişir) doğru. |
| [SetNumberFormatLinked](./setnumberformatlinked/) | Sayı biçimi hücrelere bağlıysa (etiketlerdeki sayı biçimi hücrelerde değiştiğinde değişir) doğru. |
| [ApplyFont](./applyfont/) | Veri etiketlerinin yazı tipini tüm alt düğümlere uygula. |
| [GetFont](./getfont/) | DataLabels'in yazı tipini alır; |
| [GetSeparatorType](./getseparatortype/) | Grafikteki veri etiketleri için kullanılan ayırıcı tipini alır veya ayarlar. |
| [SetSeparatorType](./setseparatortype/) | Grafikteki veri etiketleri için kullanılan ayırıcı tipini alır veya ayarlar. |
| [GetSeparatorValue](./getseparatorvalue/) | Bir grafikte veri etiketleri için kullanılan ayırıcı değerini alır veya ayarlar. |
| [SetSeparatorValue](./setseparatorvalue/) | Bir grafikte veri etiketleri için kullanılan ayırıcı değerini alır veya ayarlar. |
| [GetPosition](./getposition/) | Veri etiketinin konumunu temsil eder. |
| [SetPosition](./setposition/) | Veri etiketinin konumunu temsil eder. |
| [IsNeverOverlap](./isneveroverlap/) | Bir Pasta Grafiğini görüntüye dönüştürürken Datalabels'in hiç çakışmamasını gösterir. Not: Bu özellik yalnızca bir Pasta Grafiği görüntüye dönüştürüldüğünde anlamlıdır. |
| [SetIsNeverOverlap](./setisneveroverlap/) | Bir Pasta Grafiğini görüntüye dönüştürürken Datalabels'in hiç çakışmamasını gösterir. Not: Bu özellik yalnızca bir Pasta Grafiği görüntüye dönüştürüldüğünde anlamlıdır. |
| [GetShapeType](./getshapetype/) | Veri etiketinin şekil tipini alır veya ayarlar. |
| [SetShapeType](./setshapetype/) | Veri etiketinin şekil tipini alır veya ayarlar. |
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
| [GetTextOptions](./gettextoptions/) | Metnin seçeneklerini alır ve ayarlar. |
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
| [GetLinkedSource](./getlinkedsource/) | Çalışma sayfasına bir referansı alır ve ayarlar. |
| [SetLinkedSource](./setlinkedsource/) | Çalışma sayfasına bir referansı alır ve ayarlar. |

---
title: "Eksen Sınıfı"
linktitle: "Eksen"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Eksen sınıfı. Go'da ekseni temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/axis/
---

## Axis class

Bir çizelgenin eksenini temsil eden nesneyi kapsüller.

```go

type Axis struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetArea](./getarea/) | Alanı alır. |
| [IsAutomaticMinValue](./isautomaticminvalue/) | Minimum değerin otomatik olarak atanıp atanmadığını gösterir. |
| [SetIsAutomaticMinValue](./setisautomaticminvalue/) | Minimum değerin otomatik olarak atanıp atanmadığını gösterir. |
| [GetMinValue](./getminvalue/) | Değer eksenindeki minimum değeri temsil eder. |
| [SetMinValue](./setminvalue/) | Değer eksenindeki minimum değeri temsil eder. |
| [IsAutomaticMaxValue](./isautomaticmaxvalue/) | Maksimum değerin otomatik olarak atanıp atanmadığını gösterir. |
| [SetIsAutomaticMaxValue](./setisautomaticmaxvalue/) | Maksimum değerin otomatik olarak atanıp atanmadığını gösterir. |
| [GetMaxValue](./getmaxvalue/) | Değer eksenindeki maksimum değeri temsil eder. |
| [SetMaxValue](./setmaxvalue/) | Değer eksenindeki maksimum değeri temsil eder. |
| [IsAutomaticMajorUnit](./isautomaticmajorunit/) | Eksenin ana biriminin otomatik olarak atanıp atanmadığını gösterir. |
| [SetIsAutomaticMajorUnit](./setisautomaticmajorunit/) | Eksenin ana biriminin otomatik olarak atanıp atanmadığını gösterir. |
| [GetMajorUnit](./getmajorunit/) | Eksen için ana birimleri temsil eder. |
| [SetMajorUnit](./setmajorunit/) | Eksen için ana birimleri temsil eder. |
| [IsAutomaticMinorUnit](./isautomaticminorunit/) | Eksenin yan biriminin otomatik olarak atanıp atanmadığını gösterir. |
| [SetIsAutomaticMinorUnit](./setisautomaticminorunit/) | Eksenin yan biriminin otomatik olarak atanıp atanmadığını gösterir. |
| [GetMinorUnit](./getminorunit/) | Eksen için yan birimleri temsil eder. |
| [SetMinorUnit](./setminorunit/) | Eksen için yan birimleri temsil eder. |
| [GetAxisLine](./getaxisline/) | Bir eksenin görünümünü alır. |
| [GetMajorTickMark](./getmajortickmark/) | Belirtilen eksen için ana işaretçenin tipini temsil eder. |
| [SetMajorTickMark](./setmajortickmark/) | Belirtilen eksen için ana işaretçenin tipini temsil eder. |
| [GetMinorTickMark](./getminortickmark/) | Belirtilen eksen için yan işaretçenin tipini temsil eder. |
| [SetMinorTickMark](./setminortickmark/) | Belirtilen eksen için yan işaretçenin tipini temsil eder. |
| [GetTickLabelPosition](./getticklabelposition/) | Belirtilen eksende işaretçi etiketlerinin konumunu temsil eder. |
| [SetTickLabelPosition](./setticklabelposition/) | Belirtilen eksende işaretçi etiketlerinin konumunu temsil eder. |
| [GetCrossAt](./getcrossat/) | Kategori ekseninin değer eksenini kestiği noktayı temsil eder. |
| [SetCrossAt](./setcrossat/) | Kategori ekseninin değer eksenini kestiği noktayı temsil eder. |
| [GetCrossType](./getcrosstype/) | Diğer eksenin kesiştiği belirtilen eksende CrossType'ı temsil eder. |
| [SetCrossType](./setcrosstype/) | Diğer eksenin kesiştiği belirtilen eksende CrossType'ı temsil eder. |
| [GetLogBase](./getlogbase/) | Logaritmik tabanı temsil eder. Varsayılan değer 10'dur. |
| [SetLogBase](./setlogbase/) | Logaritmik tabanı temsil eder. Varsayılan değer 10'dur. |
| [IsLogarithmic](./islogarithmic/) | Değer ekseni ölçek tipinin logaritmik olup olmadığını temsil eder. |
| [SetIsLogarithmic](./setislogarithmic/) | Değer ekseni ölçek tipinin logaritmik olup olmadığını temsil eder. |
| [IsPlotOrderReversed](./isplotorderreversed/) | Microsoft Excel'in veri noktalarını sonundan başına doğru çizip çizmediğini temsil eder. |
| [SetIsPlotOrderReversed](./setisplotorderreversed/) | Microsoft Excel'in veri noktalarını sonundan başına doğru çizip çizmediğini temsil eder. |
| [GetAxisBetweenCategories](./getaxisbetweencategories/) | Değer ekseninin, kategori eksenini kategoriler arasında kesip kesmediğini temsil eder. |
| [SetAxisBetweenCategories](./setaxisbetweencategories/) | Değer ekseninin, kategori eksenini kategoriler arasında kesip kesmediğini temsil eder. |
| [GetTickLabels](./getticklabels/) | Belirtilen eksen için tik işareti etiketlerini temsil eden bir TickLabels nesnesi döndürür. |
| [GetTickLabelSpacing](./getticklabelspacing/) | Tik işareti etiketleri arasındaki kategori veya seri sayısını temsil eder. Yalnızca kategori ve seri eksenlerine uygulanır. |
| [SetTickLabelSpacing](./setticklabelspacing/) | Tik işareti etiketleri arasındaki kategori veya seri sayısını temsil eder. Yalnızca kategori ve seri eksenlerine uygulanır. |
| [IsAutoTickLabelSpacing](./isautoticklabelspacing/) | Tik etiketi aralığının otomatik olup olmadığını gösterir |
| [SetIsAutoTickLabelSpacing](./setisautoticklabelspacing/) | Tik etiketi aralığının otomatik olup olmadığını gösterir |
| [GetTickMarkSpacing](./gettickmarkspacing/) | Tik işaretleri arasındaki kategori veya seri sayısını döndürür veya ayarlar. Yalnızca kategori ve seri eksenlerine uygulanır. |
| [SetTickMarkSpacing](./settickmarkspacing/) | Tik işaretleri arasındaki kategori veya seri sayısını döndürür veya ayarlar. Yalnızca kategori ve seri eksenlerine uygulanır. |
| [GetDisplayUnit](./getdisplayunit/) | Belirtilen eksen için birim etiketini temsil eder. |
| [SetDisplayUnit](./setdisplayunit/) | Belirtilen eksen için birim etiketini temsil eder. |
| [GetCustomDisplayUnit](./getcustomdisplayunit/) | Görüntü birimi için özel bir değer belirtir. |
| [SetCustomDisplayUnit](./setcustomdisplayunit/) | Görüntü birimi için özel bir değer belirtir. |
| [GetDisplayUnitLabel](./getdisplayunitlabel/) | Belirtilen grafikte bir eksen üzerindeki birim etiketini temsil eder. Birim etiketleri büyük değerleri grafiklemek için faydalıdır - örneğin, milyonlar veya milyarlar halinde. |
| [IsDisplayUnitLabelShown](./isdisplayunitlabelshown/) | Görüntü birimi etiketinin belirtilen eksende gösterilip gösterilmediğini temsil eder. |
| [SetIsDisplayUnitLabelShown](./setisdisplayunitlabelshown/) | Görüntü birimi etiketinin belirtilen eksende gösterilip gösterilmediğini temsil eder. |
| [GetTitle](./gettitle/) | Bu eksenin grafikteki başlığını alır. |
| [GetCategoryType](./getcategorytype/) | Kategori ekseninin tipini temsil eder. |
| [SetCategoryType](./setcategorytype/) | Kategori ekseninin tipini temsil eder. |
| [GetBaseUnitScale](./getbaseunitscale/) | Kategori ekseni için temel birim ölçeğini temsil eder. |
| [SetBaseUnitScale](./setbaseunitscale/) | Kategori ekseni için temel birim ölçeğini temsil eder. |
| [GetMajorUnitScale](./getmajorunitscale/) | Kategori ekseni için ana birim ölçeğini temsil eder. |
| [SetMajorUnitScale](./setmajorunitscale/) | Kategori ekseni için ana birim ölçeğini temsil eder. |
| [GetMinorUnitScale](./getminorunitscale/) | Kategori ekseni için ana birim ölçeğini temsil eder. |
| [SetMinorUnitScale](./setminorunitscale/) | Kategori ekseni için ana birim ölçeğini temsil eder. |
| [IsVisible](./isvisible/) | Eksenin görünür olup olmadığını temsil eder. |
| [SetIsVisible](./setisvisible/) | Eksenin görünür olup olmadığını temsil eder. |
| [GetMajorGridLines](./getmajorgridlines/) | Bir grafik eksenindeki ana ızgara çizgilerini temsil eder. |
| [GetMinorGridLines](./getminorgridlines/) | Bir grafik eksenindeki yan ızgara çizgilerini temsil eder. |
| [GetHasMultiLevelLabels](./gethasmultilevellabels/) | Etiketlerin çok seviyeli olarak gösterilip gösterilmeyeceğini belirtir. |
| [SetHasMultiLevelLabels](./sethasmultilevellabels/) | Etiketlerin çok seviyeli olarak gösterilip gösterilmeyeceğini belirtir. |
| [GetAxisTexts](./getaxistexts/) | Chart.Calculate() yöntemi çağrıldıktan sonra eksenin etiketlerini alır. |
| [GetBins](./getbins/) | Bir grafik (Histogram/Pareto) eksenindeki kutucukları temsil eder |

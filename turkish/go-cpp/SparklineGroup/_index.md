---
title: "SparklineGroup Sınıfı"
linktitle: "SparklineGroup"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "SparklineGroup sınıfı. Go'da sparklinegroup'u temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/sparklinegroup/
---

## SparklineGroup class

<see cref="Sparkline"/> bir sparkline grubuna düzenlenir. Bir SparklineGroup, değişken sayıda sparkline öğesi içerir. Bir sparkline grubu, sparkline'ların türünü, görüntü ayarlarını ve eksen ayarlarını belirtir.

```go

type SparklineGroup struct  {
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
| [ResetRanges](./resetranges/) | Veri aralığını ve konum aralığını sparkline grubunda sıfırlar. Bu yöntem, gruptaki orijinal sparkline öğelerini temizleyecek ve yeni aralıklar için yeni sparkline öğeleri oluşturacaktır. |
| [GetPresetStyle](./getpresetstyle/) | Sparkline grubunun önceden ayarlanmış stil türünü alır ve ayarlar. |
| [SetPresetStyle](./setpresetstyle/) | Sparkline grubunun önceden ayarlanmış stil türünü alır ve ayarlar. |
| [GetSparklines](./getsparklines/) | Sparkline nesnesi koleksiyonunu alır. |
| [GetType](./gettype/) | Sparkline grubunun sparkline türünü gösterir. |
| [SetType](./settype/) | Sparkline grubunun sparkline türünü gösterir. |
| [GetPlotEmptyCellsType](./getplotemptycellstype/) | Boş hücrelerin nasıl çizileceğini gösterir. |
| [SetPlotEmptyCellsType](./setplotemptycellstype/) | Boş hücrelerin nasıl çizileceğini gösterir. |
| [GetDisplayHidden](./getdisplayhidden/) | Gizli satır ve sütunlardaki verilerin gösterilip gösterilmeyeceğini belirtir. |
| [SetDisplayHidden](./setdisplayhidden/) | Gizli satır ve sütunlardaki verilerin gösterilip gösterilmeyeceğini belirtir. |
| [GetShowHighPoint](./getshowhighpoint/) | Sparkline grubundaki verilerin en yüksek noktalarını vurgulayıp vurgulanmayacağını belirtir. |
| [SetShowHighPoint](./setshowhighpoint/) | Sparkline grubundaki verilerin en yüksek noktalarını vurgulayıp vurgulanmayacağını belirtir. |
| [GetHighPointColor](./gethighpointcolor/) | Sparkline grubundaki verilerin en yüksek noktalarının rengini alır ve ayarlar. |
| [SetHighPointColor](./sethighpointcolor/) | Sparkline grubundaki verilerin en yüksek noktalarının rengini alır ve ayarlar. |
| [GetShowLowPoint](./getshowlowpoint/) | Sparkline grubundaki verilerin en düşük noktalarını vurgulayıp vurgulanmayacağını belirtir. |
| [SetShowLowPoint](./setshowlowpoint/) | Sparkline grubundaki verilerin en düşük noktalarını vurgulayıp vurgulanmayacağını belirtir. |
| [GetLowPointColor](./getlowpointcolor/) | Sparkline grubundaki verilerin en düşük noktalarının rengini alır ve ayarlar. |
| [SetLowPointColor](./setlowpointcolor/) | Sparkline grubundaki verilerin en düşük noktalarının rengini alır ve ayarlar. |
| [GetShowNegativePoints](./getshownegativepoints/) | Sparkline grubundaki negatif değerleri farklı bir renk veya işaretçiyle vurgulayıp vurgulanmayacağını belirtir. |
| [SetShowNegativePoints](./setshownegativepoints/) | Sparkline grubundaki negatif değerleri farklı bir renk veya işaretçiyle vurgulayıp vurgulanmayacağını belirtir. |
| [GetNegativePointsColor](./getnegativepointscolor/) | Sparkline grubundaki negatif değerlerin rengini alır ve ayarlar. |
| [SetNegativePointsColor](./setnegativepointscolor/) | Sparkline grubundaki negatif değerlerin rengini alır ve ayarlar. |
| [GetShowFirstPoint](./getshowfirstpoint/) | Sparkline grubundaki verinin ilk noktasını vurgulayıp vurgulanmayacağını belirtir. |
| [SetShowFirstPoint](./setshowfirstpoint/) | Sparkline grubundaki verinin ilk noktasını vurgulayıp vurgulanmayacağını belirtir. |
| [GetFirstPointColor](./getfirstpointcolor/) | Sparkline grubundaki verinin ilk noktasının rengini alır ve ayarlar. |
| [SetFirstPointColor](./setfirstpointcolor/) | Sparkline grubundaki verinin ilk noktasının rengini alır ve ayarlar. |
| [GetShowLastPoint](./getshowlastpoint/) | Sparkline grubundaki verinin son noktasını vurgulayıp vurgulanmayacağını belirtir. |
| [SetShowLastPoint](./setshowlastpoint/) | Sparkline grubundaki verinin son noktasını vurgulayıp vurgulanmayacağını belirtir. |
| [GetLastPointColor](./getlastpointcolor/) | Sparkline grubundaki verinin son noktasının rengini alır ve ayarlar. |
| [SetLastPointColor](./setlastpointcolor/) | Sparkline grubundaki verinin son noktasının rengini alır ve ayarlar. |
| [GetShowMarkers](./getshowmarkers/) | Sparkline grubundaki her satır sparkline'deki her noktayı vurgulayıp vurgulanmayacağını belirtir. |
| [SetShowMarkers](./setshowmarkers/) | Sparkline grubundaki her satır sparkline'deki her noktayı vurgulayıp vurgulanmayacağını belirtir. |
| [GetMarkersColor](./getmarkerscolor/) | Sparkline grubundaki her satır sparkline'deki noktaların rengini alır ve ayarlar. |
| [SetMarkersColor](./setmarkerscolor/) | Sparkline grubundaki her satır sparkline'deki noktaların rengini alır ve ayarlar. |
| [GetSeriesColor](./getseriescolor/) | Sparkline grubundaki sparklineların rengini alır ve ayarlar. |
| [SetSeriesColor](./setseriescolor/) | Sparkline grubundaki sparklineların rengini alır ve ayarlar. |
| [GetPlotRightToLeft](./getplotrighttoleft/) | Çizim verisinin sağdan sola olup olmadığını belirtir. |
| [SetPlotRightToLeft](./setplotrighttoleft/) | Çizim verisinin sağdan sola olup olmadığını belirtir. |
| [GetLineWeight](./getlineweight/) | Sparkline grubundaki her satır sparkline'deki çizgi kalınlığını, puan biriminde alır ve ayarlar. |
| [SetLineWeight](./setlineweight/) | Sparkline grubundaki her satır sparkline'deki çizgi kalınlığını, puan biriminde alır ve ayarlar. |
| [GetHorizontalAxisColor](./gethorizontalaxiscolor/) | Sparklines grubundaki yatay eksenin rengini alır ve ayarlar. |
| [SetHorizontalAxisColor](./sethorizontalaxiscolor/) | Sparklines grubundaki yatay eksenin rengini alır ve ayarlar. |
| [GetShowHorizontalAxis](./getshowhorizontalaxis/) | Sparklines yatay ekseninin gösterilip gösterilmeyeceğini belirtir.Yatay eksen, sparkline sıfır eksenini geçen veri içeriyorsa görünür. |
| [SetShowHorizontalAxis](./setshowhorizontalaxis/) | Sparklines yatay ekseninin gösterilip gösterilmeyeceğini belirtir.Yatay eksen, sparkline sıfır eksenini geçen veri içeriyorsa görünür. |
| [GetHorizontalAxisDateRange](./gethorizontalaxisdaterange/) | Sparklines verileri için tarih değerlerini içeren aralığı temsil eder. |
| [SetHorizontalAxisDateRange](./sethorizontalaxisdaterange/) | Sparklines verileri için tarih değerlerini içeren aralığı temsil eder. |
| [GetVerticalAxisMaxValueType](./getverticalaxismaxvaluetype/) | Dikey eksenin maksimum değer tipini temsil eder. |
| [SetVerticalAxisMaxValueType](./setverticalaxismaxvaluetype/) | Dikey eksenin maksimum değer tipini temsil eder. |
| [GetVerticalAxisMaxValue](./getverticalaxismaxvalue/) | Dikey eksen için özel maksimum değeri alır ve ayarlar. |
| [SetVerticalAxisMaxValue_Double](./setverticalaxismaxvalue_double/) | Dikey eksen için özel maksimum değeri alır ve ayarlar. |
| [SetVerticalAxisMaxValue_SparklineAxisMinMaxType_Double](./setverticalaxismaxvalue_sparklineaxisminmaxtype_double/) | Belirtilen eksen değer tipiyle sparkline dikey ekseni için özel maksimum değeri ayarlar. |
| [SetVerticalAxisMinValue_SparklineAxisMinMaxType_Double](./setverticalaxisminvalue_sparklineaxisminmaxtype_double/) | Belirtilen eksen değer tipiyle sparkline dikey ekseni için özel minimum değeri ayarlar. |
| [GetVerticalAxisMinValueType](./getverticalaxisminvaluetype/) | Dikey eksenin minimum değer tipini temsil eder. |
| [SetVerticalAxisMinValueType](./setverticalaxisminvaluetype/) | Dikey eksenin minimum değer tipini temsil eder. |
| [GetVerticalAxisMinValue](./getverticalaxisminvalue/) | Dikey eksen için özel minimum değeri alır ve ayarlar. |
| [SetVerticalAxisMinValue_Double](./setverticalaxisminvalue_double/) | Dikey eksen için özel minimum değeri alır ve ayarlar. |

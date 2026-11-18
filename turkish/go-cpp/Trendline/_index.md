---
title: "Trendline Sınıfı"
linktitle: "Trendline"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Trendline sınıfı. Go dilinde trendline nesnesini temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/trendline/
---

## Trendline class

Bir grafikteki trend çizgisini temsil eder.

```go

type Trendline struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewTrendline](./newtrendline/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [IsNameAuto](./isnameauto/) | Microsoft Excel'in trend çizgisinin adını otomatik olarak belirleyip belirlemediğini döndürür. |
| [SetIsNameAuto](./setisnameauto/) | Microsoft Excel'in trend çizgisinin adını otomatik olarak belirleyip belirlemediğini döndürür. |
| [GetType](./gettype/) | Trend çizgisi tipini döndürür. |
| [GetName](./getname/) | Trend çizgisinin adını döndürür. |
| [SetName](./setname/) | Trend çizgisinin adını döndürür. |
| [GetOrder](./getorder/) | Trend çizgisi tipi Polinom olduğunda trend çizgisi sırasını (1'den büyük bir tam sayı) alır veya ayarlar. Sıra 2 ile 6 arasında olmalıdır. |
| [SetOrder](./setorder/) | Trend çizgisi tipi Polinom olduğunda trend çizgisi sırasını (1'den büyük bir tam sayı) alır veya ayarlar. Sıra 2 ile 6 arasında olmalıdır. |
| [GetPeriod](./getperiod/) | Hareketli ortalama trend çizgisi için periyodu alır veya ayarlar. |
| [SetPeriod](./setperiod/) | Hareketli ortalama trend çizgisi için periyodu alır veya ayarlar. |
| [GetForward](./getforward/) | Trend çizgisinin ileri doğru uzadığı dönem (veya dağılım grafiğindeki birimler) sayısını alır veya ayarlar. Dönem sayısı sıfır veya daha büyük olmalıdır. |
| [SetForward](./setforward/) | Trend çizgisinin ileri doğru uzadığı dönem (veya dağılım grafiğindeki birimler) sayısını alır veya ayarlar. Dönem sayısı sıfır veya daha büyük olmalıdır. |
| [GetBackward](./getbackward/) | Trend çizgisinin geriye doğru uzadığı dönem (veya dağılım grafiğindeki birimler) sayısını alır veya ayarlar. Dönem sayısı sıfır veya daha büyük olmalıdır. Grafik tipi sütun ise, dönem sayısı 0 ile 0,5 arasında olmalıdır. |
| [SetBackward](./setbackward/) | Trend çizgisinin geriye doğru uzadığı dönem (veya dağılım grafiğindeki birimler) sayısını alır veya ayarlar. Dönem sayısı sıfır veya daha büyük olmalıdır. Grafik tipi sütun ise, dönem sayısı 0 ile 0,5 arasında olmalıdır. |
| [GetDisplayEquation](./getdisplayequation/) | Trend çizgisi denkleminin grafikte (R-kare değeriyle aynı veri etiketi içinde) gösterilip gösterilmediğini temsil eder. Bu özelliği True olarak ayarlamak, veri etiketlerini otomatik olarak açar. |
| [SetDisplayEquation](./setdisplayequation/) | Trend çizgisi denkleminin grafikte (R-kare değeriyle aynı veri etiketi içinde) gösterilip gösterilmediğini temsil eder. Bu özelliği True olarak ayarlamak, veri etiketlerini otomatik olarak açar. |
| [GetDisplayRSquared](./getdisplayrsquared/) | Trend çizgisinin R-kare değerinin grafikte (denklemle aynı veri etiketi içinde) gösterilip gösterilmediğini temsil eder. Bu özelliği True olarak ayarlamak, veri etiketlerini otomatik olarak açar. |
| [SetDisplayRSquared](./setdisplayrsquared/) | Trend çizgisinin R-kare değerinin grafikte (denklemle aynı veri etiketi içinde) gösterilip gösterilmediğini temsil eder. Bu özelliği True olarak ayarlamak, veri etiketlerini otomatik olarak açar. |
| [GetIntercept](./getintercept/) | Trend çizgisinin değer eksenini kestiği noktayı alır veya ayarlar. |
| [SetIntercept](./setintercept/) | Trend çizgisinin değer eksenini kestiği noktayı alır veya ayarlar. |
| [GetDataLabels](./getdatalabels/) | Belirtilen seri için DataLabels nesnesini temsil eder. |
| [GetLegendEntry](./getlegendentry/) | Bu trend çizgisine göre lejand girişini alır |
| [GetCompoundType](./getcompoundtype/) | Bileşik çizgi tipini belirtir. |
| [SetCompoundType](./setcompoundtype/) | Bileşik çizgi tipini belirtir. |
| [GetDashType](./getdashtype/) | Kesikli çizgi tipini belirtir |
| [SetDashType](./setdashtype/) | Kesikli çizgi tipini belirtir |
| [GetCapType](./getcaptype/) | Bitiş kapaklarını belirtir. |
| [SetCapType](./setcaptype/) | Bitiş kapaklarını belirtir. |
| [GetJoinType](./getjointype/) | Birleştirme kapaklarını belirtir. |
| [SetJoinType](./setjointype/) | Birleştirme kapaklarını belirtir. |
| [GetBeginType](./getbegintype/) | Bir çizginin başlangıcı için ok ucunu belirtir. |
| [SetBeginType](./setbegintype/) | Bir çizginin başlangıcı için ok ucunu belirtir. |
| [GetEndType](./getendtype/) | Bir çizginin sonu için ok ucunu belirtir. |
| [SetEndType](./setendtype/) | Bir çizginin sonu için ok ucunu belirtir. |
| [GetBeginArrowLength](./getbeginarrowlength/) | Bir çizginin başlangıcı için ok ucunun uzunluğunu belirtir. |
| [SetBeginArrowLength](./setbeginarrowlength/) | Bir çizginin başlangıcı için ok ucunun uzunluğunu belirtir. |
| [GetEndArrowLength](./getendarrowlength/) | Bir çizginin sonu için ok ucunun uzunluğunu belirtir. |
| [SetEndArrowLength](./setendarrowlength/) | Bir çizginin sonu için ok ucunun uzunluğunu belirtir. |
| [GetBeginArrowWidth](./getbeginarrowwidth/) | Bir çizginin başlangıcı için ok ucunun genişliğini belirtir. |
| [SetBeginArrowWidth](./setbeginarrowwidth/) | Bir çizginin başlangıcı için ok ucunun genişliğini belirtir. |
| [GetEndArrowWidth](./getendarrowwidth/) | Bir çizginin sonu için ok ucunun genişliğini belirtir. |
| [SetEndArrowWidth](./setendarrowwidth/) | Bir çizginin sonu için ok ucunun genişliğini belirtir. |
| [GetThemeColor](./getthemecolor/) | Tema rengini alır ve ayarlar. |
| [SetThemeColor](./setthemecolor/) | Tema rengini alır ve ayarlar. |
| [GetColor](./getcolor/) | Çizginin rengini temsil eder. |
| [SetColor](./setcolor/) | Çizginin rengini temsil eder. |
| [GetTransparency](./gettransparency/) | Çizginin şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |
| [SetTransparency](./settransparency/) | Çizginin şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |
| [GetStyle](./getstyle/) | Çizginin stilini temsil eder. |
| [SetStyle](./setstyle/) | Çizginin stilini temsil eder. |
| [GetWeight](./getweight/) | Çizginin WeightType değerini alır veya ayarlar. |
| [SetWeight](./setweight/) | Çizginin WeightType değerini alır veya ayarlar. |
| [GetWeightPt](./getweightpt/) | Çizginin ağırlığını puan biriminde alır veya ayarlar. |
| [SetWeightPt](./setweightpt/) | Çizginin ağırlığını puan biriminde alır veya ayarlar. |
| [GetWeightPx](./getweightpx/) | Çizginin ağırlığını piksel biriminde alır veya ayarlar. |
| [SetWeightPx](./setweightpx/) | Çizginin ağırlığını piksel biriminde alır veya ayarlar. |
| [GetFormattingType](./getformattingtype/) | Biçim tipini alır veya ayarlar. |
| [SetFormattingType](./setformattingtype/) | Biçim tipini alır veya ayarlar. |
| [IsAutomaticColor](./isautomaticcolor/) | Çizginin renginin otomatik atanıp atanmadığını gösterir. |
| [IsVisible](./isvisible/) | Çizginin görünür olup olmadığını temsil eder. |
| [SetIsVisible](./setisvisible/) | Çizginin görünür olup olmadığını temsil eder. |
| [IsAuto](./isauto/) | Bu çizgi stilinin otomatik atanıp atanmadığını gösterir. |
| [SetIsAuto](./setisauto/) | Bu çizgi stilinin otomatik atanıp atanmadığını gösterir. |
| [GetGradientFill](./getgradientfill/) | Gradyan dolguyu temsil eder. |

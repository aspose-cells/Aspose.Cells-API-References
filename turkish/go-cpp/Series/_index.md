---
title: "Series Sınıfı"
linktitle: "Series"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Series sınıfı. Go'da series'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/series/
---

## Series class

Bir grafikteki tek bir veri serisini temsil eden nesneyi kapsüller.

```go

type Series struct  {
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
| [IsFiltered](./isfiltered/) | Serinin seçili mi yoksa filtrelenmiş mi olduğunu belirtir. True, bu series'in filtrelendiğini ve grafikte gösterilmeyeceğini gösterir. |
| [SetIsFiltered](./setisfiltered/) | Serinin seçili mi yoksa filtrelenmiş mi olduğunu belirtir. True, bu series'in filtrelendiğini ve grafikte gösterilmeyeceğini gösterir. |
| [GetLayoutProperties](./getlayoutproperties/) | Düzenin özelliklerini temsil eder. |
| [Move](./move/) | Series'i yukarı veya aşağı hareket ettirir. |
| [GetPoints](./getpoints/) | Grafikte bir series içindeki nokta koleksiyonunu alır. |
| [GetArea](./getarea/) | Series nesnesinin arka plan alanını temsil eder. |
| [GetBorder](./getborder/) | Bir Series nesnesinin kenarını temsil eder. |
| [GetName](./getname/) | Veri serisinin adını alır veya ayarlar. |
| [SetName](./setname/) | Veri serisinin adını alır veya ayarlar. |
| [GetDisplayName](./getdisplayname/) | Grafik üzerinde gösterilen serinin adını alır. |
| [GetCountOfDataValues](./getcountofdatavalues/) | Veri değerlerinin sayısını alır. |
| [IsVerticalValues](./isverticalvalues/) | Veri kaynağının dikey olup olmadığını gösterir. |
| [GetValues](./getvalues/) | Bu grafik serisinin Y değerlerini temsil eder. |
| [SetValues](./setvalues/) | Bu grafik serisinin Y değerlerini temsil eder. |
| [GetPointValues](./getpointvalues/) | Bu serinin grafikteki her noktasını çizmek için kullanılan gerçek değerleri alır. |
| [GetCategoryValues](./getcategoryvalues/) | Bu serinin grafikteki her noktasını çizmek için kullanılan gerçek kategori değerlerini alır. |
| [GetValuesFormatCode](./getvaluesformatcode/) | Values NumberList'in format kodunu temsil eder. |
| [SetValuesFormatCode](./setvaluesformatcode/) | Values NumberList'in format kodunu temsil eder. |
| [GetXValuesFormatCode](./getxvaluesformatcode/) | X Values'ın NumberList'inin format kodunu temsil eder. |
| [SetXValuesFormatCode](./setxvaluesformatcode/) | X Values'ın NumberList'inin format kodunu temsil eder. |
| [GetXValues](./getxvalues/) | Bu grafik serisinin X değerlerini temsil eder. |
| [SetXValues](./setxvalues/) | Bu grafik serisinin X değerlerini temsil eder. |
| [GetBubbleSizes](./getbubblesizes/) | Grafik serisinin balon boyutu değerlerini alır veya ayarlar. |
| [SetBubbleSizes](./setbubblesizes/) | Grafik serisinin balon boyutu değerlerini alır veya ayarlar. |
| [GetTrendLines](./gettrendlines/) | Bu serinin tüm trend çizgilerini döndürür. |
| [GetSmooth](./getsmooth/) | Eğri yumuşatmayı temsil eder. Çizgi grafiği veya dağılım grafiği için eğri yumuşatma açıksa doğru. Yalnızca çizgi grafiklerinde ve çizgili dağılım grafiklerinde uygulanır. |
| [SetSmooth](./setsmooth/) | Eğri yumuşatmayı temsil eder. Çizgi grafiği veya dağılım grafiği için eğri yumuşatma açıksa doğru. Yalnızca çizgi grafiklerinde ve çizgili dağılım grafiklerinde uygulanır. |
| [GetShadow](./getshadow/) | Serinin gölgesi varsa doğru. |
| [SetShadow](./setshadow/) | Serinin gölgesi varsa doğru. |
| [GetHas3DEffect](./gethas3deffect/) | Serinin üç boyutlu bir görünümü varsa doğru. |
| [SetHas3DEffect](./sethas3deffect/) | Serinin üç boyutlu bir görünümü varsa doğru. |
| [GetBar3DShapeType](./getbar3dshapetype/) | 3D çubuk veya sütun grafiğiyle kullanılan 3D şekil tipini alır veya ayarlar. |
| [SetBar3DShapeType](./setbar3dshapetype/) | 3D çubuk veya sütun grafiğiyle kullanılan 3D şekil tipini alır veya ayarlar. |
| [GetDataLabels](./getdatalabels/) | Belirtilen ASeries için DataLabels nesnesini temsil eder. |
| [GetType](./gettype/) | Bir veri serisinin tipini alır veya ayarlar. |
| [SetType](./settype/) | Bir veri serisinin tipini alır veya ayarlar. |
| [GetMarker](./getmarker/) | Marker'ı alır</see>. |
| [GetPlotOnSecondAxis](./getplotonsecondaxis/) | Bu serinin ikinci değer ekseninde çizilip çizilmediğini gösterir. |
| [SetPlotOnSecondAxis](./setplotonsecondaxis/) | Bu serinin ikinci değer ekseninde çizilip çizilmediğini gösterir. |
| [GetXErrorBar](./getxerrorbar/) | Serinin X yönündeki hata çubuğunu temsil eder. |
| [GetYErrorBar](./getyerrorbar/) | Serinin Y yönündeki hata çubuğunu temsil eder. |
| [GetHasHiLoLines](./gethashilolines/) | Çizgi grafiğinin yüksek-düşük çizgileri varsa doğru. Yalnızca çizgi grafiklerinde uygulanır. |
| [SetHasHiLoLines](./sethashilolines/) | Çizgi grafiğinin yüksek-düşük çizgileri varsa doğru. Yalnızca çizgi grafiklerinde uygulanır. |
| [GetHiLoLines](./gethilolines/) | Bir çizgi grafiğindeki seri için yüksek-düşük çizgileri temsil eden HiLoLines nesnesini döndürür. Yalnızca çizgi grafiklerinde uygulanır. |
| [GetHasSeriesLines](./gethasserieslines/) | Yığılmış sütun grafik veya çubuk grafik serileri çizgilerine sahipse veya bir Pie of Pie grafiği ya da Bar of Pie grafiği iki bölüm arasında bağlayıcı çizgilere sahipse doğru. Yalnızca yığılmış sütun grafikler, çubuk grafikler, Pie of Pie grafikler veya Bar of Pie grafikler için geçerlidir. |
| [SetHasSeriesLines](./sethasserieslines/) | Yığılmış sütun grafik veya çubuk grafik serileri çizgilerine sahipse veya bir Pie of Pie grafiği ya da Bar of Pie grafiği iki bölüm arasında bağlayıcı çizgilere sahipse doğru. Yalnızca yığılmış sütun grafikler, çubuk grafikler, Pie of Pie grafikler veya Bar of Pie grafikler için geçerlidir. |
| [GetSeriesLines](./getserieslines/) | Yığılmış çubuk grafik veya yığılmış sütun grafik için seri çizgilerini temsil eden bir SeriesLines nesnesi döndürür. Yalnızca yığılmış çubuk ve yığılmış sütun grafikler için geçerlidir. |
| [GetHasDropLines](./gethasdroplines/) | Grafiğin düşen çizgileri varsa doğru. Yalnızca çizgi grafik veya alan grafikler için geçerlidir. |
| [SetHasDropLines](./sethasdroplines/) | Grafiğin düşen çizgileri varsa doğru. Yalnızca çizgi grafik veya alan grafikler için geçerlidir. |
| [GetDropLines](./getdroplines/) | Çizgi grafik veya alan grafik üzerindeki bir serinin düşen çizgilerini temsil eden bir Line nesnesi döndürür. Yalnızca çizgi grafikler veya alan grafikler için geçerlidir. |
| [GetHasUpDownBars](./gethasupdownbars/) | Bir çizgi grafiğinde yukarı ve aşağı çubuklar varsa doğru. Yalnızca çizgi grafikler için geçerlidir. |
| [SetHasUpDownBars](./sethasupdownbars/) | Bir çizgi grafiğinde yukarı ve aşağı çubuklar varsa doğru. Yalnızca çizgi grafikler için geçerlidir. |
| [GetUpBars](./getupbars/) | Bir çizgi grafiğindeki yukarı çubukları temsil eden bir DropBars nesnesi döndürür. Yalnızca çizgi grafikler için geçerlidir. |
| [GetDownBars](./getdownbars/) | Bir çizgi grafiğindeki aşağı çubukları temsil eden bir DropBars nesnesi döndürür. Yalnızca çizgi grafikler için geçerlidir. |
| [IsColorVaried](./iscolorvaried/) | Nokta renklerinin değişken olup olmadığını temsil eder. Grafik yalnızca bir seri içermeli veya bu grafik bir pasta grafiği olmalıdır. |
| [SetIsColorVaried](./setiscolorvaried/) | Nokta renklerinin değişken olup olmadığını temsil eder. Grafik yalnızca bir seri içermeli veya bu grafik bir pasta grafiği olmalıdır. |
| [GetGapWidth](./getgapwidth/) | Sütun veya çubuk kümeleri arasındaki boşluğu, çubuk veya sütun genişliğinin yüzdesi olarak döndürür veya ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır. |
| [SetGapWidth](./setgapwidth/) | Sütun veya çubuk kümeleri arasındaki boşluğu, çubuk veya sütun genişliğinin yüzdesi olarak döndürür veya ayarlar. Bu özelliğin değeri 0 ile 500 arasında olmalıdır. |
| [GetFirstSliceAngle](./getfirstsliceangle/) | İlk pasta grafiği veya halka grafiği diliminin açısını derece cinsinden alır veya ayarlar (dikeyden saat yönünde). Yalnızca pasta, 3D pasta ve halka grafikler için geçerlidir; değerler 0 ile 360 arasındadır. |
| [SetFirstSliceAngle](./setfirstsliceangle/) | İlk pasta grafiği veya halka grafiği diliminin açısını derece cinsinden alır veya ayarlar (dikeyden saat yönünde). Yalnızca pasta, 3D pasta ve halka grafikler için geçerlidir; değerler 0 ile 360 arasındadır. |
| [GetOverlap](./getoverlap/) | Çubukların ve sütunların nasıl konumlandırıldığını belirtir. -100 ile 100 arasında bir değer olabilir. Yalnızca 2D çubuk ve 2D sütun grafikler için geçerlidir. |
| [SetOverlap](./setoverlap/) | Çubukların ve sütunların nasıl konumlandırıldığını belirtir. -100 ile 100 arasında bir değer olabilir. Yalnızca 2D çubuk ve 2D sütun grafikler için geçerlidir. |
| [GetSecondPlotSize](./getsecondplotsize/) | Bir pie of pie grafiği veya bar of pie grafiğinin ikincil bölümünün boyutunu, birincil pasta boyutunun yüzde olarak döndürür veya ayarlar. 5 ile 200 arasında bir değer olabilir. |
| [SetSecondPlotSize](./setsecondplotsize/) | Bir pie of pie grafiği veya bar of pie grafiğinin ikincil bölümünün boyutunu, birincil pasta boyutunun yüzde olarak döndürür veya ayarlar. 5 ile 200 arasında bir değer olabilir. |
| [GetSplitType](./getsplittype/) | Bir pie of pie veya bar of pie grafiğinde ikinci pasta veya çubuğun hangi veri noktalarını içereceğini belirlemek için bir değer döndürür veya ayarlar. |
| [SetSplitType](./setsplittype/) | Bir pie of pie veya bar of pie grafiğinde ikinci pasta veya çubuğun hangi veri noktalarını içereceğini belirlemek için bir değer döndürür veya ayarlar. |
| [GetSplitValue](./getsplitvalue/) | Bir pie of pie veya bar of pie grafiğinde ikinci pasta veya çubuğun hangi veri noktalarını içereceğini belirlemek için kullanılacak bir değer döndürür veya ayarlar. |
| [SetSplitValue](./setsplitvalue/) | Bir pie of pie veya bar of pie grafiğinde ikinci pasta veya çubuğun hangi veri noktalarını içereceğini belirlemek için kullanılacak bir değer döndürür veya ayarlar. |
| [IsAutoSplit](./isautosplit/) | Eşik değerinin otomatik olup olmadığını gösterir. |
| [GetBubbleScale](./getbubblescale/) | Belirtilen grafik grubundaki balonların ölçek faktörünü alır veya ayarlar. 0 (sıfır) ile 300 arasında bir tam sayı değer olabilir ve varsayılan boyutun yüzdesine karşılık gelir. Yalnızca balon grafikler için geçerlidir. |
| [SetBubbleScale](./setbubblescale/) | Belirtilen grafik grubundaki balonların ölçek faktörünü alır veya ayarlar. 0 (sıfır) ile 300 arasında bir tam sayı değer olabilir ve varsayılan boyutun yüzdesine karşılık gelir. Yalnızca balon grafikler için geçerlidir. |
| [GetSizeRepresents](./getsizerepresents/) | Balon grafiğinde balon boyutunun neyi temsil ettiğini alır veya ayarlar. |
| [SetSizeRepresents](./setsizerepresents/) | Balon grafiğinde balon boyutunun neyi temsil ettiğini alır veya ayarlar. |
| [GetShowNegativeBubbles](./getshownegativebubbles/) | Grafik grubu için negatif balonlar gösteriliyorsa doğru. Yalnızca balon grafikler için geçerlidir. |
| [SetShowNegativeBubbles](./setshownegativebubbles/) | Grafik grubu için negatif balonlar gösteriliyorsa doğru. Yalnızca balon grafikler için geçerlidir. |
| [GetDoughnutHoleSize](./getdoughnutholesize/) | Bir halka grafik grubundaki deliğin boyutunu döndürür veya ayarlar. Delik boyutu, grafik boyutunun yüzde olarak 10 ile 90 arasında ifade edilir. |
| [SetDoughnutHoleSize](./setdoughnutholesize/) | Bir halka grafik grubundaki deliğin boyutunu döndürür veya ayarlar. Delik boyutu, grafik boyutunun yüzde olarak 10 ile 90 arasında ifade edilir. |
| [GetExplosion](./getexplosion/) | Açık bir pasta diliminin pasta grafiğinin merkezinden uzaklığı, pasta çapının yüzde olarak ifade edilir. |
| [SetExplosion](./setexplosion/) | Açık bir pasta diliminin pasta grafiğinin merkezinden uzaklığı, pasta çapının yüzde olarak ifade edilir. |
| [GetHasRadarAxisLabels](./gethasradaraxislabels/) | Bir radar grafiğinde kategori ekseni etiketleri varsa doğru. Yalnızca radar grafikler için geçerlidir. |
| [SetHasRadarAxisLabels](./sethasradaraxislabels/) | Bir radar grafiğinde kategori ekseni etiketleri varsa doğru. Yalnızca radar grafikler için geçerlidir. |
| [GetHasLeaderLines](./gethasleaderlines/) | Serinin lider çizgileri varsa doğru. |
| [SetHasLeaderLines](./sethasleaderlines/) | Serinin lider çizgileri varsa doğru. |
| [GetLeaderLines](./getleaderlines/) | Grafikte lider çizgileri temsil eder. Lider çizgileri veri etiketlerini veri noktalarına bağlar. Bu nesne bir koleksiyon değildir; tek bir lider çizgiyi temsil eden bir nesne yoktur. |
| [GetLegendEntry](./getlegendentry/) | Bu seriye göre lejand girişini alır. |
| [GetShapeProperties](./getshapeproperties/) | Serinin görsel şekil özelliklerini tutan ShapePropertyCollection nesnesini alır. |

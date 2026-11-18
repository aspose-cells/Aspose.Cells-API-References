---
title: "Walls Sınıfı"
linktitle: "Walls"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Walls sınıfı. Go içinde duvarları temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/walls/
---

## Walls class

3D grafik duvarlarını temsil eden nesneyi kapsüller.

```go

type Walls struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewWalls](./newwalls/) | Bir üst nesneden oluşturur. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetCenterX](./getcenterx/) | Chart.Calculate() yöntemi çağrıldıktan sonra duvar merkezinin sol-alt köşesinin x koordinatını, grafiğin genişliğinin 1/4000 birimi cinsinden alır. |
| [GetCenterY](./getcentery/) | Chart.Calculate() yöntemi çağrıldıktan sonra duvar merkezinin sol-alt köşesinin y koordinatını, grafiğin yüksekliğinin 1/4000 birimi cinsinden alır. |
| [GetWidth](./getwidth/) | Chart.Calculate() yöntemi çağrıldıktan sonra soldan sağa genişliği, grafiğin genişliğinin 1/4000 birimi cinsinden alır. |
| [GetDepth](./getdepth/) | Chart.Calculate() yöntemi çağrıldıktan sonra önden arkaya derinliği, grafiğin genişliğinin 1/4000 birimi cinsinden alır. |
| [GetHeight](./getheight/) | Chart.Calculate() yöntemi çağrıldıktan sonra üstten alta yüksekliği, grafiğin yüksekliğinin 1/4000 birimi cinsinden alır. |
| [GetCenterXPx](./getcenterxpx/) | Chart.Calculate() yöntemi çağrıldıktan sonra duvar merkezinin alt-sol köşesinin x koordinatını piksel biriminde alır. |
| [GetCenterYPx](./getcenterypx/) | Chart.Calculate() yöntemi çağrıldıktan sonra duvar merkezinin sol-alt köşesinin y koordinatını piksel biriminde alır. |
| [GetWidthPx](./getwidthpx/) | Chart.Calculate() yöntemi çağrıldıktan sonra soldan sağa genişliği piksel biriminde alır. |
| [GetDepthPx](./getdepthpx/) | Chart.Calculate() yöntemi çağrıldıktan sonra önden arkaya derinliği piksel biriminde alır. |
| [GetHeightPx](./getheightpx/) | Chart.Calculate() metodunu çağırdıktan sonra piksel biriminde üstten alta yüksekliği alır. |
| [GetCubePointCount](./getcubepointcount/) | Chart.Calculate() metodunu çağırdıktan sonra küp noktalarının sayısını alır. |
| [GetCubePointXPx](./getcubepointxpx/) | Chart.Calculate() metodunu çağırdıktan sonra duvar küpünün tepe noktasının x koordinatını alır. Duvar küpünün tepe noktası sayısı sekizdir. |
| [GetCubePointYPx](./getcubepointypx/) | Chart.Calculate() metodunu çağırdıktan sonra duvar küpünün tepe noktasının y koordinatını alır. Duvar küpünün tepe noktası sayısı sekizdir. |
| [GetBackgroundColor](./getbackgroundcolor/) | Alan'ın arka plan rengini alır veya ayarlar. |
| [SetBackgroundColor](./setbackgroundcolor/) | Alan'ın arka plan rengini alır veya ayarlar. |
| [GetForegroundColor](./getforegroundcolor/) | Ön plan rengini alır veya ayarlar. |
| [SetForegroundColor](./setforegroundcolor/) | Ön plan rengini alır veya ayarlar. |
| [GetFormatting](./getformatting/) | Alan'ın biçimlendirmesini temsil eder. |
| [SetFormatting](./setformatting/) | Alan'ın biçimlendirmesini temsil eder. |
| [GetInvertIfNegative](./getinvertifnegative/) | Özellik true ise ve grafik noktasının değeri negatif bir sayı ise, ön plan rengi ve arka plan rengi değiştirilecektir. |
| [SetInvertIfNegative](./setinvertifnegative/) | Özellik true ise ve grafik noktasının değeri negatif bir sayı ise, ön plan rengi ve arka plan rengi değiştirilecektir. |
| [GetFillFormat](./getfillformat/) | Belirtilen grafik veya şekil için doldurma biçimlendirme özelliklerini içeren bir FillFormat nesnesini temsil eder. |
| [GetTransparency](./gettransparency/) | Alanının şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |
| [SetTransparency](./settransparency/) | Alanının şeffaflık derecesini 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak döndürür veya ayarlar. |
| [GetBorder](./getborder/) | Sınır Çizgisini alır veya ayarlar. |
| [SetBorder](./setborder/) | Sınır Çizgisini alır veya ayarlar. |

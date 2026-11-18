---
title: "SeriesCollection Sınıfı"
linktitle: "SeriesCollection"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "SeriesCollection sınıfı. Go'da seriescollection'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/seriescollection/
---

## SeriesCollection class

Bir <see cref="Series"/> nesnelerinin bir koleksiyonunu kapsüller.

```go

type SeriesCollection struct  {
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
| [Get](./get/) | Belirtilen indeksteki Series öğesini alır. |
| [GetSeriesByOrder](./getseriesbyorder/) | Sıra ile Series öğesini alır. |
| [RemoveAt](./removeat/) | Belirli bir indeksteki seriyi kaldır. |
| [GetCategoryData](./getcategorydata/) | Kategori eksen değerlerinin aralığını alır veya ayarlar. Bu, hücre aralığı (örneğin "d1:e10") veya değer dizisi (örneğin "{2,6,8,10}") olabilir. |
| [SetCategoryData](./setcategorydata/) | Kategori eksen değerlerinin aralığını alır veya ayarlar. Bu, hücre aralığı (örneğin "d1:e10") veya değer dizisi (örneğin "{2,6,8,10}") olabilir. |
| [GetSecondCategoryData](./getsecondcategorydata/) | İkinci kategori eksen değerlerinin aralığını alır veya ayarlar. Bu, hücre aralığı (örneğin "d1:e10") veya değer dizisi (örneğin "{2,6,8,10}") olabilir. Yalnızca bazı seriler ikinci eksende çizildiğinde etkili olur. |
| [SetSecondCategoryData](./setsecondcategorydata/) | İkinci kategori eksen değerlerinin aralığını alır veya ayarlar. Bu, hücre aralığı (örneğin "d1:e10") veya değer dizisi (örneğin "{2,6,8,10}") olabilir. Yalnızca bazı seriler ikinci eksende çizildiğinde etkili olur. |
| [SwapSeries](./swapseries/) | İki serinin sırasını doğrudan değiştirir. |
| [SetSeriesNames](./setseriesnames/) | Grafikteki tüm serilerin adlarını ayarlar. |
| [AddR1C1](./addr1c1/) | Series koleksiyonunu bir grafiğe ekler. |
| [Add_String_Bool](./add_string_bool/) | Series koleksiyonunu bir grafiğe ekler. |
| [Add_String_Bool_Bool](./add_string_bool_bool/) | Series koleksiyonunu bir grafiğe ekler. |
| [IsColorVaried](./iscolorvaried/) | Noktaların renginin değişken olup olmadığını temsil eder. |
| [SetIsColorVaried](./setiscolorvaried/) | Noktaların renginin değişken olup olmadığını temsil eder. |
| [Clear](./clear/) | Koleksiyonu temizler |
| [ChangeColors](./changecolors/) | Grafik serileri için Tek Renkli Paleti ayarlar. |
| [GetCount](./getcount/) | Örnekte bulunan öğe sayısını alır. |

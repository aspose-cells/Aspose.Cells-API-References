---
title: "PivotFieldCollection Sınıfı"
linktitle: "PivotFieldCollection"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "PivotFieldCollection sınıfı. Go'da pivotfieldcollection'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/pivotfieldcollection/
---

## PivotFieldCollection class

Pivot tablonun farklı bölgelerindeki tüm PivotField nesnelerinin koleksiyonunu temsil eder.

```go

type PivotFieldCollection struct  {
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
| [GetType](./gettype/) | PivotFields türünü alır. |
| [Get_Int](./get_int/) | Belirli indeksteki PivotField nesnesini alır. |
| [Get_String](./get_string/) | Belirli isimdeki PivotField nesnesini alır. |
| [RemoveAt](./removeat/) | Alanı indeksine göre kaldırır. Yalnızca filtre, satır, sütun, veri bölgesi için. |
| [AddByBaseIndex](./addbybaseindex/) | Belirli tip PivotFields'e bir PivotField nesnesi ekler. |
| [Add](./add/) | Belirli tip PivotFields'e bir PivotField nesnesi ekler. |
| [Insert](./insert/) | Belirli indekse bir pivot alanı ekler. |
| [Clear](./clear/) | PivotFieldCollection içindeki tüm alanları temizle |
| [Remove](./remove/) | Mevcut bölgeden alanı kaldırır. |
| [Move](./move/) | PivotField'i mevcut konumdan hedef konuma taşır |
| [GetCount](./getcount/) | Örnekte bulunan öğe sayısını alır. |

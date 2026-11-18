---
title: "ColumnCollection Sınıfı"
linktitle: "ColumnCollection"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "ColumnCollection sınıfı. Go'da columncollection'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/columncollection/
---

## ColumnCollection class

Bir çalışma sayfasındaki bireysel sütun (ayar)larını temsil eden <see cref="Column"/> nesnelerinin koleksiyonu. Column nesnesi yalnızca sütun genişliği, stiller vb. gibi tüm sütun için ayarları temsil eder, ilgili sütunda boş olmayan hücrelerin (veri) olup olmamasıyla ilgisi yoktur. Ve bu koleksiyonun "Count" özelliği yalnızca bu koleksiyonda örneklenmiş Column nesnelerinin sayısını temsil eder, çalışma sayfasında boş olmayan hücrelerin (veri) olup olmamasıyla ilgisi yoktur.

```go

type ColumnCollection struct  {
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
| [GetColumnByIndex](./getcolumnbyindex/) | Listedeki konuma göre Column nesnesini alır. |
| [Get](./get/) | Sütun indeksine göre bir Column nesnesi alır. Verilen sütun indeksi için Column nesnesi, daha önce mevcut değilse oluşturulur. |
| [GetCount](./getcount/) | Örnekte bulunan öğe sayısını alır. |

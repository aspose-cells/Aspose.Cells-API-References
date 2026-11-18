---
title: "RowCollection Sınıfı"
linktitle: "RowCollection"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "RowCollection sınıfı. Go dilinde rowcollection'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/rowcollection/
---

## RowCollection class

Bir çalışma sayfasındaki bireysel satırları temsil eden <see cref="Row"/> nesnelerini toplar.

```go

type RowCollection struct  {
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
| [GetCount](./getcount/) | Bu koleksiyondaki satır sayısını alır. |
| [GetEnumerator](./getenumerator/) | Bu koleksiyon içinde satırları yineleyen bir enumeratör alır |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | Bu koleksiyon içinde satırları yineleyen bir enumeratör alır |
| [GetRowByIndex](./getrowbyindex/) | Listedeki konuma göre satır nesnesini alır. |
| [Get](./get/) | Verilen satır indeksine göre bir Row nesnesi alır. Verilen satır indeksi için Row nesnesi daha önce yoksa oluşturulur. |
| [Clear](./clear/) | Tüm satırları ve hücreleri temizle. |
| [RemoveAt](./removeat/) | Bu koleksiyondaki belirtilen indeks (konum) konumundaki satır öğesini kaldır. |

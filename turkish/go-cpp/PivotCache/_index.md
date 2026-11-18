---
title: "PivotCache Sınıfı"
linktitle: "PivotCache"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "PivotCache sınıfı. Go'da pivotcache'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/pivotcache/
---

## PivotCache class

Bazı PivotTable raporları için bellek önbelleğini temsil eder.

```go

type PivotCache struct  {
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
| [GetMissingItemsLimit](./getmissingitemslimit/) | Kullanılmayan öğeleri atamadan önce izin verilecek kullanılmayan öğe sayısını alır ve ayarlar. Bu değer -2'den büyük ve 1048577'den küçük olmalıdır. PivotCacheMissingItemsLimitConst; |
| [SetMissingItemsLimit](./setmissingitemslimit/) | Kullanılmayan öğeleri atamadan önce izin verilecek kullanılmayan öğe sayısını alır ve ayarlar. Bu değer -2'den büyük ve 1048577'den küçük olmalıdır. PivotCacheMissingItemsLimitConst; |
| [Refresh_PivotTableRefreshOption](./refresh_pivottablerefreshoption/) | Veri kaynağından verileri yeniler ve bu pivot önbelleği veri kaynağı olan tüm pivottable'ların görünümü için verileri hesaplar. |
| [Refresh](./refresh/) | Veri kaynağından verileri yeniler ve bu pivot önbelleği veri kaynağı olan tüm pivottable'ların görünümü için verileri hesaplar. |
| [GetPivotTables](./getpivottables/) | Bu pivot önbelleğiyle tüm pivot tablolarını alır. |
| [Dispose](./dispose/) | Tüm kaynakları serbest bırak. |
| [GetSourceType](./getsourcetype/) | PivotTableSourceType'ı alır. |

---
title: "Sınıf PivotCache"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotCache sınıfı. Bazı PivotTable raporları için bellek önbelleğini temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivotcache/
---
## PivotCache class

Bazı PivotTable raporları için bellek önbelleğini temsil eder.

```csharp
public abstract class PivotCache : IDisposable
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [MissingItemsLimit](../../aspose.cells.pivot/pivotcache/missingitemslimit/) { get; set; } | Kullanılmayan öğeleri atamadan önce izin verilecek kullanılmayan öğe sayısını alır ve ayarlar. Bu değer -2'den büyük ve 1048577'den küçük olmalıdır. [`PivotCacheMissingItemsLimitConst`](../pivotcachemissingitemslimitconst/); |
| abstract [SourceType](../../aspose.cells.pivot/pivotcache/sourcetype/) { get; } | [`PivotTableSourceType`](../pivottablesourcetype/) değerini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| abstract [Dispose](../../aspose.cells.pivot/pivotcache/dispose/)() | Tüm kaynakları serbest bırak. |
| [GetPivotTables](../../aspose.cells.pivot/pivotcache/getpivottables/)() | Bu pivot önbelleğine sahip tüm pivot tabloları al. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh)() | Veri kaynağından verileri yeniler ve veri kaynağı bu pivot önbelleği olan tüm pivot tablolarının görünümü için verileri hesaplar. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh_1)(PivotTableRefreshOption) | Veri kaynağından verileri yeniler ve veri kaynağı bu pivot önbelleği olan tüm pivot tablolarının görünümü için verileri hesaplar. |

### Açıklamalar

Tüm veriler bu önbellekte toplanacak ve pivot tablo yalnızca bu önbellekten veri alacak, veri kaynağına doğrudan erişmeyecek. Bazı [`PivotTable`](../pivottable/)ların veri kaynağı aynıysa, bir pivot önbelleği kullanacaklar.

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)



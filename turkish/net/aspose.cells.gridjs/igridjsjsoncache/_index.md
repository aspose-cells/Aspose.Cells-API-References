---
title: "Arayüz IGridJsJsonCache"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridJs.IGridJsJsonCache arayüzü. JSON önbellek arayüzü, müşterilerin belirli depolama ve geçersiz kılma stratejilerini uygulamasını sağlar"
type: docs
url: /tr/net/aspose.cells.gridjs/igridjsjsoncache/
---
## IGridJsJsonCache interface

JSON önbellek arayüzü - müşteriler belirli depolama ve geçersiz kılma stratejileri uygular

```csharp
public interface IGridJsJsonCache
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ClearAll](../../aspose.cells.gridjs/igridjsjsoncache/clearall/)() | Tüm önbellekleri temizle |
| [GetCacheKey](../../aspose.cells.gridjs/igridjsjsoncache/getcachekey/)(string, string) | Bir önbellek anahtarı oluştur. Müşteriler iş gereksinimlerine göre uid'yi dahil edip etmeyeceklerine karar verebilir. - Yalnızca dosya adı önemliyse: uid'yi yok say ve sadece fileName'i kullan (önerilir, aynı dosya için önbellek paylaşımına izin verir). - Aynı ada sahip dosyaları ayırt etmek gerekiyorsa: uid'yi kullan (katı mod). |
| [Invalidate](../../aspose.cells.gridjs/igridjsjsoncache/invalidate/)(string) | Belirtilen önbellek girdisini geçersiz kıl. |
| [InvalidateAllForUid](../../aspose.cells.gridjs/igridjsjsoncache/invalidateallforuid/)(string) | Belirtilen uid'yi içeren tüm önbellek girdilerini geçersiz kıl. Bu, önbellekleme için kullanılan tam fileName'i bilmediğinizde faydalıdır. |
| [SetJson](../../aspose.cells.gridjs/igridjsjsoncache/setjson/)(string, string) | JSON'ı önbelleğe yaz. |
| [TryGetJson](../../aspose.cells.gridjs/igridjsjsoncache/trygetjson/)(string) | JSON'ı önbellekten almaya çalış. |

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)



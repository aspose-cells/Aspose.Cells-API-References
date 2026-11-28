---
title: "IGridJsJsonCache.GetCacheKey"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IGridJsJsonCache yöntemi. Bir önbellek anahtarı oluştur. Müşteriler, iş gereksinimlerine göre uid'yi dahil edip etmeyeceklerine karar verebilir. Yalnızca dosya adı önemliyse uid'yi görmezden gel ve sadece fileName'i kullan; bu, aynı dosya için önbellek paylaşımına izin verir. Aynı ada sahip dosyaları ayırt etmek gerekiyorsa uid sıkı modda kullanılmalıdır."
type: docs
url: /tr/net/aspose.cells.gridjs/igridjsjsoncache/getcachekey/
---
## IGridJsJsonCache.GetCacheKey method

Bir önbellek anahtarı oluştur. Müşteriler iş gereksinimlerine göre uid'yi dahil edip etmeyeceklerine karar verebilir. - Yalnızca dosya adı önemliyse: uid'yi yok say ve sadece fileName'i kullan (önerilir, aynı dosya için önbellek paylaşımına izin verir). - Aynı ada sahip dosyaları ayırt etmek gerekiyorsa: uid'yi kullan (katı mod).

```csharp
public string GetCacheKey(string uid, string fileName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | String | Dosyanın benzersiz tanımlayıcısı (yükleme başına farklı olabilir) |
| fileName | String | Orijinal dosya adı |

### Dönüş Değeri

Önbellek anahtarı

### Ayrıca Bakınız

* interface [IGridJsJsonCache](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)



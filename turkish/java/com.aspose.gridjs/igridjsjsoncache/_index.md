---
title: "IGridJsJsonCache"
second_title: "Aspose.Cells for Java API Referansı"
description: "JSON önbellek arayüzü - müşteriler belirli depolama ve geçersiz kılma stratejileri uygular."
type: docs
url: /tr/java/com.aspose.gridjs/igridjsjsoncache/
---
```
public interface IGridJsJsonCache
```

JSON önbellek arayüzü - müşteriler belirli depolama ve geçersiz kılma stratejileri uygular.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [clearAll()](#clearAll--) | Tüm önbellekleri temizle |
| [getCacheKey(String uid, String fileName)](#getCacheKey-java.lang.String-java.lang.String-) | Bir önbellek anahtarı oluştur. |
| [invalidate(String cacheKey)](#invalidate-java.lang.String-) | Belirtilen önbellek girişini geçersiz kıl. |
| [invalidateAllForUid(String uid)](#invalidateAllForUid-java.lang.String-) | Belirtilen uid'yi içeren tüm önbellek girdilerini geçersiz kıl. |
| [setJson(String cacheKey, String json)](#setJson-java.lang.String-java.lang.String-) | JSON'ı önbelleğe yazın. |
| [tryGetJson(String cacheKey)](#tryGetJson-java.lang.String-) | JSON'ı önbellekten almaya çalışın. |
### clearAll() {#clearAll--}
```
public abstract void clearAll()
```


Tüm önbellekleri temizle

### getCacheKey(String uid, String fileName) {#getCacheKey-java.lang.String-java.lang.String-}
```
public abstract String getCacheKey(String uid, String fileName)
```


Bir önbellek anahtarı oluştur. Müşteriler, iş gereksinimlerine göre uid'yi dahil edip etmeyeceklerine karar verebilir. - Yalnızca dosya adı önemliyse: uid'yi yok say ve sadece fileName'i kullan (önerilir, aynı dosya için önbellek paylaşımına izin verir). - Aynı ada sahip dosyaları ayırt etmek gerekiyorsa: uid'yi kullan (katı mod).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosyanın benzersiz tanımlayıcısı (yükleme başına farklı olabilir) |
| fileName | java.lang.String | Orijinal dosya adı |

**Returns:**
java.lang.String - Önbellek anahtarı
### invalidate(String cacheKey) {#invalidate-java.lang.String-}
```
public abstract void invalidate(String cacheKey)
```


Belirtilen önbellek girişini geçersiz kıl.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cacheKey | java.lang.String | Önbellek anahtarı |

### invalidateAllForUid(String uid) {#invalidateAllForUid-java.lang.String-}
```
public abstract void invalidateAllForUid(String uid)
```


Belirtilen uid'yi içeren tüm önbellek girdilerini geçersiz kılın. Bu, önbellekleme için kullanılan tam dosya adını bilmediğinizde faydalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Önbellek anahtarlarında eşleşecek benzersiz tanımlayıcı |

### setJson(String cacheKey, String json) {#setJson-java.lang.String-java.lang.String-}
```
public abstract void setJson(String cacheKey, String json)
```


JSON'ı önbelleğe yazın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cacheKey | java.lang.String | Önbellek anahtarı |
| json | java.lang.String | JSON dizesi |

### tryGetJson(String cacheKey) {#tryGetJson-java.lang.String-}
```
public abstract String tryGetJson(String cacheKey)
```


JSON'ı önbellekten almaya çalışın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cacheKey | java.lang.String | Önbellek anahtarı |

**Returns:**
java.lang.String - Önbellek eşleşmesi durumunda JSON dizesi, aksi takdirde null

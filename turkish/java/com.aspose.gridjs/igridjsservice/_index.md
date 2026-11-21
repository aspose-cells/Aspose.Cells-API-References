---
title: "IGridJsService"
second_title: "Aspose.Cells for Java API Referansı"
description: "Denetleyici eylemlerinde kullanılan temel işlem API'leri arayüzünü temsil eder."
type: docs
url: /tr/java/com.aspose.gridjs/igridjsservice/
---
```
public interface IGridJsService
```

Denetleyici eylemlerinde kullanılan temel işlem API'leri arayüzünü temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | Yerel dosyadan resim ekleme işlemini uygular. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Uzak URL'den resim ekleme işlemini uygular. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Çalışma kitabı örneğinin bellek önbelleğinde olup olmadığını kontrol edin. Bu yöntem yalnızca İş Birliği modu için uygulanır. |
| [clearAllJsonCache()](#clearAllJsonCache--) | Tüm JSON önbellek girişlerini (bellek ve disk) temizler. |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | Belirtilen benzersiz kimliğe ait tüm JSON önbellek girişlerini temizler. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | Resim kopyalama işlemini uygular. |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | Belirtilen benzersiz kimliğe göre dosya için JSON dizesini alır. |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | Workbook için JSON dizesini akıma yazar |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Belirtilen benzersiz kimliğe göre dosya için JSON dizesini akıma yazar. |
| [dispose()](#dispose--) |  |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | Dosya indirme işlemini uygular |
| [getFile(String fileid)](#getFile-java.lang.String-) | Dosya akışını al |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | Resim akışını al. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | Resim URL'sini alır. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Belirtilen benzersiz kimliği kullanarak dosyadaki belirtilen sayfanın JSON dizesini önbellekten alır. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | Belirtilen benzersiz kimliği kullanarak önbellekten dosyadaki belirtilen sayfanın JSON dizesini akıma yazar.. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | Belirtilen benzersiz kimliği kullanarak önbellekten dosyanın JSON dizesini alır, JSON içinde çıktı dosya adını ayarlar. |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | Gömülü ole nesnesinin bayt dizisi verisini alır. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Güncelleme işlemini uygular. |
### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public abstract String addImage(String p, String uid, InputStream filestream)
```


Yerel dosyadan resim ekleme işlemini uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| p | java.lang.String | JSON dize parametresi |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| filestream | java.io.InputStream | Görselin filestream'i |

**Returns:**
java.lang.String - JSON dize sonucu
### addImageByURL(String p, String uid, InputStream filestream, String imageurl) {#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public abstract String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


Uzak URL'den resim ekleme işlemini uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| p | java.lang.String | JSON dize parametresi |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| filestream | java.io.InputStream | Görselin filestream'i |
| imageurl | java.lang.String | Görsel URL'sini belirtin. |

**Returns:**
java.lang.String - JSON dize sonucu
### checkInCacheForCollaborative(String uid) {#checkInCacheForCollaborative-java.lang.String-}
```
public abstract boolean checkInCacheForCollaborative(String uid)
```


Çalışma kitabı örneğinin bellek önbelleğinde olup olmadığını kontrol edin. Bu yöntem yalnızca İş Birliği modu için uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String |  |

**Returns:**
boolean -
### clearAllJsonCache() {#clearAllJsonCache--}
```
public abstract void clearAllJsonCache()
```


Tüm JSON önbellek girişlerini (bellek ve disk) temizler.

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public abstract void clearJsonCacheForUid(String uid)
```


Belirtilen benzersiz kimliğe ait tüm JSON önbellek girişlerini temizler. Kaynak dosyayı dışarıdan değiştirdikten sonra bunu çağırın, böylece bir sonraki istek JSON'u yeniden oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public abstract String copyImage(String p, String uid)
```


Resim kopyalama işlemini uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| p | java.lang.String | JSON dize parametresi |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |

**Returns:**
java.lang.String - JSON dize sonucu
### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public abstract StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


Belirtilen benzersiz kimliğe göre dosya için JSON dizesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Dosya yolu |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public abstract void detailStreamJson(OutputStream stream, String filePath)
```


Workbook için JSON dizesini akıma yazar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Yazılacak akış |
| filePath | java.lang.String | Dosya yolu |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public abstract void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


Belirtilen benzersiz kimliğe göre dosya için JSON dizesini akıma yazar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Yazılacak akış |
| filePath | java.lang.String | Dosya yolu |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |

### dispose() {#dispose--}
```
public abstract void dispose()
```




### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public abstract String download(String p, String uid, String filename)
```


Dosya indirme işlemini uygular

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| p | java.lang.String | JSON parametresi |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| dosya adı | java.lang.String | Dosya adı |

**Returns:**
java.lang.String - Dosya URL'si
### getFile(String fileid) {#getFile-java.lang.String-}
```
public abstract InputStream getFile(String fileid)
```


Dosya akışını al

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileid | java.lang.String | dosya kimliği |

**Returns:**
java.io.InputStream - Dosyanın akışı
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public abstract InputStream image(String uid, String picid)
```


Resim akışını al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| picid | java.lang.String | Görsel kimliği. |

**Returns:**
java.io.InputStream - Görsel akışı
### imageUrl(String baseURL, String picid, String uid) {#imageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public abstract String imageUrl(String baseURL, String picid, String uid)
```


Resim URL'sini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| baseURL | java.lang.String | Temel eylem URL'si. |
| picid | java.lang.String | Görsel kimliği. |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |

**Returns:**
java.lang.String - Görüntü URL'si
### lazyLoadingJson(String sheetName, String uid) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public abstract StringBuilder lazyLoadingJson(String sheetName, String uid)
```


Belirtilen benzersiz kimliği kullanarak dosyadaki belirtilen sayfanın JSON dizesini önbellekten alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetName | java.lang.String | sayfa adı. |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |

**Returns:**
java.lang.StringBuilder
### lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid) {#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public abstract void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
```


Belirtilen benzersiz kimliği kullanarak önbellekten dosyadaki belirtilen sayfanın JSON dizesini akıma yazar..

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Yazılacak akış |
| sheetName | java.lang.String | Sayfa adı. |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |

### load(String uid, String filename) {#load-java.lang.String-java.lang.String-}
```
public abstract String load(String uid, String filename)
```


Belirtilen benzersiz kimliği kullanarak önbellekten dosyanın JSON dizesini alır, JSON içinde çıktı dosya adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| dosya adı | java.lang.String | JSON içinde dosya adını belirtir. Null olarak ayarlanırsa, varsayılan dosya adı: book1. |

**Returns:**
java.lang.String - JSON dizesi
### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public abstract byte[] ole(String uid, String sheetname, int oleid, String label)
```


Gömülü ole nesnesinin bayt dizisi verisini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| sheetname | java.lang.String | Çalışma sayfası adı. |
| oleid | int | Gömülü ole nesnesi için kimlik. |
| label | java.lang.String | Gömülü ole nesnesinin görüntü etiketi. |

**Returns:**
byte[] - Gömülü ole nesnesinin bayt dizisi verisi.
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public abstract String updateCell(String p, String uid)
```


Güncelleme işlemini uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| p | java.lang.String | Güncelleme işleminin JSON biçim dizesi. |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |

**Returns:**
java.lang.String

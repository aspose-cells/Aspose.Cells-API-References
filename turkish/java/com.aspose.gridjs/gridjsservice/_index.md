---
title: "GridJsService"
second_title: "Aspose.Cells for Java API Referansı"
description: "Denetleyici eylemlerinde kullanılan temel işlem API'lerini sağlar."
type: docs
url: /tr/java/com.aspose.gridjs/gridjsservice/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.gridjs.IGridJsService](../../com.aspose.gridjs/igridjsservice)
```
public class GridJsService implements IGridJsService
```

Denetleyici eylemlerinde kullanılan temel işlem API'lerini sağlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GridJsService(GridJsOptions options)](#GridJsService-com.aspose.gridjs.GridJsOptions-) | GridJsService için varsayılan yapıcı |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addImage(String p, String uid, InputStream filestream)](#addImage-java.lang.String-java.lang.String-java.io.InputStream-) | Yerel dosyadan resim ekleme işlemini uygular. |
| [addImageByURL(String p, String uid, InputStream filestream, String imageurl)](#addImageByURL-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Yerel dosyadan resim ekleme işlemini uygular. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Çalışma kitabı örneğinin bellek önbelleğinde olup olmadığını kontrol edin. Bu yöntem yalnızca İş Birliği modu için uygulanır. |
| [clearAllJsonCache()](#clearAllJsonCache--) | Tüm JSON önbellek girişlerini (bellek ve disk) temizler. |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | Belirtilen benzersiz kimliğe ait tüm JSON önbellek girişlerini temizler. |
| [copyImage(String p, String uid)](#copyImage-java.lang.String-java.lang.String-) | Resim kopyalama işlemini uygular. |
| [destroy()](#destroy--) | Bu yöntem yalnızca Java içindir, DisposableBean içinde yok etme metodunu uygular, istek tamamlandığında Spring tarafından otomatik olarak çağrılır, aslında Dispose metodunu çağırır. |
| [detailFileJsonWithUid(String filePath, String uid)](#detailFileJsonWithUid-java.lang.String-java.lang.String-) | Belirtilen benzersiz kimliğe göre dosya için JSON dizesini alır. |
| [detailStreamJson(OutputStream stream, String filePath)](#detailStreamJson-java.io.OutputStream-java.lang.String-) | Dosya için JSON dizesini akıma yazar. |
| [detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)](#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Belirtilen benzersiz kimliğe göre dosya için JSON dizesini akıma yazar. |
| [dispose()](#dispose--) | Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [download(String p, String uid, String filename)](#download-java.lang.String-java.lang.String-java.lang.String-) | Dosya indirme işlemini uygular |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFile(String fileid)](#getFile-java.lang.String-) | Dosya akışını al |
| [getSettings()](#getSettings--) | Çalışma kitabı ayarlarını temsil eder. |
| [hashCode()](#hashCode--) |  |
| [image(String uid, String picid)](#image-java.lang.String-java.lang.String-) | Resim akışını al. |
| [imageUrl(String baseURL, String picid, String uid)](#imageUrl-java.lang.String-java.lang.String-java.lang.String-) | Resim URL'sini alır. |
| [lazyLoadingJson(String sheetName, String uid)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Belirtilen benzersiz kimliği kullanarak dosyadaki belirtilen sayfanın JSON dizesini önbellekten alır. |
| [lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)](#lazyLoadingStreamJson-java.io.OutputStream-java.lang.String-java.lang.String-) | Belirtilen benzersiz kimliği kullanarak önbellekten dosyadaki belirtilen sayfanın JSON dizesini akıma yazar.. |
| [load(String uid, String filename)](#load-java.lang.String-java.lang.String-) | Belirtilen benzersiz kimliği kullanarak önbellekten dosyanın JSON dizesini alır, JSON içinde çıktı dosya adını ayarlar. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [ole(String uid, String sheetname, int oleid, String label)](#ole-java.lang.String-java.lang.String-int-java.lang.String-) | Gömülü ole nesnesinin bayt dizisi verisini alır. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | Çalışma kitabı ayarlarını temsil eder. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | Çalışma sayfasındaki tüm dize değerlerini hedef dile çevir. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Güncelleme işlemini uygular. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsService(GridJsOptions options) {#GridJsService-com.aspose.gridjs.GridJsOptions-}
```
public GridJsService(GridJsOptions options)
```


GridJsService için varsayılan yapıcı

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [GridJsOptions](../../com.aspose.gridjs/gridjsoptions) |  |

### addImage(String p, String uid, InputStream filestream) {#addImage-java.lang.String-java.lang.String-java.io.InputStream-}
```
public String addImage(String p, String uid, InputStream filestream)
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
public String addImageByURL(String p, String uid, InputStream filestream, String imageurl)
```


Yerel dosyadan resim ekleme işlemini uygular.

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
public boolean checkInCacheForCollaborative(String uid)
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
public void clearAllJsonCache()
```


Tüm JSON önbellek girişlerini (bellek ve disk) temizler.

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


Belirtilen benzersiz kimliğe ait tüm JSON önbellek girişlerini temizler. Kaynak dosyayı dışarıdan değiştirdikten sonra bunu çağırın, böylece bir sonraki istek JSON'u yeniden oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |

### copyImage(String p, String uid) {#copyImage-java.lang.String-java.lang.String-}
```
public String copyImage(String p, String uid)
```


Resim kopyalama işlemini uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| p | java.lang.String | JSON dize parametresi |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |

**Returns:**
java.lang.String - JSON dize sonucu
### destroy() {#destroy--}
```
public void destroy()
```


Bu yöntem yalnızca Java içindir, DisposableBean içinde yok etme metodunu uygular, istek tamamlandığında Spring tarafından otomatik olarak çağrılır, aslında Dispose metodunu çağırır.

### detailFileJsonWithUid(String filePath, String uid) {#detailFileJsonWithUid-java.lang.String-java.lang.String-}
```
public StringBuilder detailFileJsonWithUid(String filePath, String uid)
```


Belirtilen benzersiz kimliğe göre dosya için JSON dizesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String | Tam dosya yolu |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |

**Returns:**
java.lang.StringBuilder
### detailStreamJson(OutputStream stream, String filePath) {#detailStreamJson-java.io.OutputStream-java.lang.String-}
```
public void detailStreamJson(OutputStream stream, String filePath)
```


Dosya için JSON dizesini akıma yazar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Yazılacak akış |
| filePath | java.lang.String | Tam dosya yolu |

### detailStreamJsonWithUid(OutputStream stream, String filePath, String uid) {#detailStreamJsonWithUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void detailStreamJsonWithUid(OutputStream stream, String filePath, String uid)
```


Belirtilen benzersiz kimliğe göre dosya için JSON dizesini akıma yazar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Yazılacak akış |
| filePath | java.lang.String | Tam dosya yolu |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |

### dispose() {#dispose--}
```
public void dispose()
```


Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür.

### download(String p, String uid, String filename) {#download-java.lang.String-java.lang.String-java.lang.String-}
```
public String download(String p, String uid, String filename)
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
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFile(String fileid) {#getFile-java.lang.String-}
```
public InputStream getFile(String fileid)
```


Dosya akışını al

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileid | java.lang.String | dosya kimliği |

**Returns:**
java.io.InputStream - Dosyanın akışı
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Çalışma kitabı ayarlarını temsil eder.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### image(String uid, String picid) {#image-java.lang.String-java.lang.String-}
```
public InputStream image(String uid, String picid)
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
public String imageUrl(String baseURL, String picid, String uid)
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
public StringBuilder lazyLoadingJson(String sheetName, String uid)
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
public void lazyLoadingStreamJson(OutputStream stream, String sheetName, String uid)
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
public String load(String uid, String filename)
```


Belirtilen benzersiz kimliği kullanarak önbellekten dosyanın JSON dizesini alır, JSON içinde çıktı dosya adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| dosya adı | java.lang.String | JSON içinde dosya adını belirtir. Null olarak ayarlanırsa, varsayılan dosya adı: book1. |

**Returns:**
java.lang.String - JSON dizesi
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### ole(String uid, String sheetname, int oleid, String label) {#ole-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] ole(String uid, String sheetname, int oleid, String label)
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
### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Çalışma kitabı ayarlarını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage) {#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-}
```
public String translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)
```


Çalışma sayfasındaki tüm dize değerlerini hedef dile çevir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| sheetName | java.lang.String | Sayfa adı |
| translator | [ITextTranslator](../../com.aspose.gridjs/itexttranslator) | Çeviri işlevini uygulayan çevirmen |
| hedefDil | java.lang.String | Hedef dil |

**Returns:**
java.lang.String -
### updateCell(String p, String uid) {#updateCell-java.lang.String-java.lang.String-}
```
public String updateCell(String p, String uid)
```


Güncelleme işlemini uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| p | java.lang.String | Güncelleme işleminin JSON biçim dizesi. |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |

**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |


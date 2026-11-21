---
title: "GridJsWorkbook"
second_title: "Aspose.Cells for Java API Referansı"
description: "GridJs için ana giriş sınıfını temsil eder."
type: docs
url: /tr/java/com.aspose.gridjs/gridjsworkbook/
---

**Inheritance:**
java.lang.Object
```
public class GridJsWorkbook
```

GridJs için ana giriş sınıfını temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GridJsWorkbook()](#GridJsWorkbook--) | GridJsWorkbook'ın yeni bir örneğini oluşturur. |
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [CacheImp](#CacheImp) | Önbellek depolama için özel uygulama, önbelleği akış şeklinde depolamak istiyorsanız, ayarlamanız ve uygulamanız gerekir. |
| [CalculateEngine](#CalculateEngine) | Hesaplama motoru için özel uygulama, özel bir hesaplama yapmak istiyorsanız, onu ayarlamanız ve uygulamanız gerekir. |
| [PICTURE_TYPE](#PICTURE-TYPE) | Görsel türü için sabit değer |
| [UpdateMonitor](#UpdateMonitor) | Güncelleme işlemini izlemek için güncelleme izleyicisini alır/ayarlar |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [burnRedactionFile(String excelFilePath, String uid)](#burnRedactionFile-java.lang.String-java.lang.String-) | Uygular (yanar) tüm kırpma işlemlerini, kırpma şekillerini ve hedef şekillerini kaldırarak veya hedef hücre aralığı içeriğini temizleyerek çalışma kitabında. |
| [checkInCacheForCollaborative(String uid)](#checkInCacheForCollaborative-java.lang.String-) | Çalışma kitabı örneğinin bellek önbelleğinde olup olmadığını kontrol edin. Bu yöntem yalnızca İş Birliği modu için uygulanır. |
| [clearAllJsonCache()](#clearAllJsonCache--) | \\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8? |
| [clearJsonCacheForUid(String uid)](#clearJsonCacheForUid-java.lang.String-) | \\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c? |
| [copyImageOrShape(String uid, String p)](#copyImageOrShape-java.lang.String-java.lang.String-) | Görüntüyü veya şekli kopyalar. |
| [dispose()](#dispose--) | Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [errorJson(String msg)](#errorJson-java.lang.String-) | JSON formatında hata mesajı dizesini alır. |
| [exportToJson()](#exportToJson--) | Bellek verisinden JSON dizesini alır, JSON içindeki varsayılan dosya adı: book1. |
| [exportToJson(String filename)](#exportToJson-java.lang.String-) | Bellek verisinden JSON dizesini alır, JSON içinde çıktı dosya adını ayarlar. |
| [exportToJsonStringBuilder(String filename)](#exportToJsonStringBuilder-java.lang.String-) | Bellek verisinden JSON dizesini alır, JSON içinde çıktı dosya adını ayarlar. |
| [exportToJsonStringBuilder(String filename, String uid)](#exportToJsonStringBuilder-java.lang.String-java.lang.String-) |  |
| [getCacheDirectory()](#getCacheDirectory--) | Elektronik tablo dosyasını depolamak için önbellek dizinini alır. |
| [getClass()](#getClass--) |  |
| [getGridLoadFormat(String extension)](#getGridLoadFormat-java.lang.String-) | Dosya uzantısına göre yükleme biçimini alır |
| [getImageStream(String uid, String picid, String cachedir)](#getImageStream-java.lang.String-java.lang.String-java.lang.String-) | Resim akışını al. |
| [getImageUrl(String uid, String picid, String delimiter)](#getImageUrl-java.lang.String-java.lang.String-java.lang.String-) | Resim URL'sini alır. |
| [getJsonByUid(String uid, String filename)](#getJsonByUid-java.lang.String-java.lang.String-) | Belirtilen benzersiz kimliği kullanarak önbellekten dosyanın JSON dizesini alır, JSON içinde çıktı dosya adını ayarlar. |
| [getOle(String uid, String sheetname, int oleid, String label)](#getOle-java.lang.String-java.lang.String-int-java.lang.String-) | Gömülü ole nesnesinin bayt dizisi verisini alır. |
| [getSettings()](#getSettings--) | Çalışma kitabı ayarlarını temsil eder. |
| [getSheetJsonWithCache(String uid, String sheetName, String fileName)](#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e sayfa \\u9428? |
| [getUidForFile(String fileName)](#getUidForFile-java.lang.String-) | Verilen dosya adını kullanarak dosya önbelleği için yeni benzersiz bir kimlik oluşturur. |
| [getWorkbookJsonWithCache(String uid, String fileName)](#getWorkbookJsonWithCache-java.lang.String-java.lang.String-) | \\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b? |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream filestream, int format)](#importExcelFile-java.io.InputStream-int-) | Excel dosyasını dosya akışından yükleme biçimiyle içe aktarır. |
| [importExcelFile(InputStream filestream, int format, String password)](#importExcelFile-java.io.InputStream-int-java.lang.String-) | Excel dosyasını dosya akışından yükleme biçimi ve açma parolasıyla içe aktarır. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Excel dosyasını dosya yolundan içe aktarır. |
| [importExcelFile(String uid, InputStream filestream, int format)](#importExcelFile-java.lang.String-java.io.InputStream-int-) | Excel dosyasını dosya akışından içe aktarır. |
| [importExcelFile(String uid, InputStream filestream, int format, String password)](#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-) | Excel dosyasını dosya akışından yükleme biçimi ve açma parolasıyla içe aktarır. |
| [importExcelFile(String uid, String fileName)](#importExcelFile-java.lang.String-java.lang.String-) | Excel dosyasını dosya yolundan içe aktarır. |
| [importExcelFile(String uid, String fileName, String password)](#importExcelFile-java.lang.String-java.lang.String-java.lang.String-) | Excel dosyasını dosya yolundan ve açma parolasıyla içe aktarır. |
| [importExcelFileFromJson(String json)](#importExcelFileFromJson-java.lang.String-) | Excel dosyasını JSON formatındaki dizeden içe aktarır. |
| [insertImage(String uid, String p, InputStream s, String imageUrl)](#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-) | Çalışma sayfasına dosya akışından veya URL'den resim ekler (dosya akışı veya URL sağlanmalıdır) veya p.type, AutoShapeType'tan biri olduğunda şekil ekler. |
| [jsonToStream(OutputStream stream, String filename)](#jsonToStream-java.io.OutputStream-java.lang.String-) | Bellekteki Workbook'tan JSON oluşturur ve belirtilen akışa yazar. |
| [jsonToStream(OutputStream stream, String filename, String uid)](#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-) |  |
| [jsonToStreamByUid(OutputStream stream, String uid, String filename)](#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-) | Belirtilen benzersiz kimliği kullanarak dosyanın JSON dizesini önbellekten alır, JSON içinde çıktı dosya adını ayarlar ve akışa yazar. |
| [lazyLoadingJson(String uid, String sheetName)](#lazyLoadingJson-java.lang.String-java.lang.String-) | Belirtilen benzersiz kimliği kullanarak dosyadaki belirtilen sayfanın JSON dizesini önbellekten alır. |
| [lazyLoadingStream(OutputStream stream, String uid, String sheetName)](#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-) | Belirtilen benzersiz kimliği kullanarak dosyadaki belirtilen sayfanın JSON dizesini önbellekten alır ve akışa yazar. |
| [mergeExcelFileFromJson(String uid, String json)](#mergeExcelFileFromJson-java.lang.String-java.lang.String-) | Bellek verisine toplu bir güncelleme uygular. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)](#redactFile-java.lang.String-java.lang.String-java.lang.String---) | JSON işlemleri dizisine dayanarak bir Excel dosyasında redaksiyon gerçekleştirir. |
| [saveToCacheWithFileName(String uid, String filename, String password)](#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-) | Bellek verisini belirtilen dosya adıyla önbellek dosyasına kaydeder ve ayrıca açma parolasını ayarlar, kaydetme biçimi dosya adının uzantısına göre belirlenir. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | Bellek verisini sream'e kaydeder, orijinal dosya biçimine göre belirlenir. |
| [saveToExcelFile(String path)](#saveToExcelFile-java.lang.String-) | Bellek verisini dosya yoluna kaydeder, dosyanın uzantısı varsa kaydetme biçimi dosya uzantısına göre belirlenir. |
| [saveToHtml(OutputStream stream)](#saveToHtml-java.io.OutputStream-) | Bellek verisini sream'e kaydeder, kaydetme biçimi html'dir. |
| [saveToHtml(String path)](#saveToHtml-java.lang.String-) | Bellek verisini dosya yoluna kaydeder, kaydetme biçimi html'dir. |
| [saveToPdf(OutputStream stream)](#saveToPdf-java.io.OutputStream-) | Bellek verisini sream'e kaydeder, kaydetme biçimi pdf'dir. |
| [saveToPdf(String path)](#saveToPdf-java.lang.String-) | Bellek verilerini dosya yoluna kaydeder, kaydetme formatı pdf. |
| [saveToXlsx(OutputStream stream)](#saveToXlsx-java.io.OutputStream-) | Bellek verilerini akışa kaydeder, kaydetme formatı xlsx. |
| [saveToXlsx(String path)](#saveToXlsx-java.lang.String-) | Bellek verilerini dosya yoluna kaydeder, kaydetme formatı xlsx. |
| [setCacheDirectory(String value)](#setCacheDirectory-java.lang.String-) | Elektronik tablo dosyasını depolamak için önbellek dizinini ayarlar. |
| [setImageUrlBase(String baseImageURL)](#setImageUrlBase-java.lang.String-) | Denetleyiciden temel görüntü alma eylemi URL'sini ayarla. |
| [setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)](#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-) | Yükleme işlemi için InterruptMonitor'ı ayarlar. |
| [setInterruptMonitorForSave(GridInterruptMonitor monitor)](#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-) | Kaydetme işlemi için InterruptMonitor'ı ayarlar. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridjs.GridWorkbookSettings-) | Çalışma kitabı ayarlarını temsil eder. |
| [setTransParentView(String excelFilePath, String uid, boolean isTransparent)](#setTransParentView-java.lang.String-java.lang.String-boolean-) | Çalışma kitabındaki redaksiyon şekillerinin saydamlığını ayarlar. |
| [toString()](#toString--) |  |
| [translateSheetAsync(String uid, String sheetName, ITextTranslator translator, String targetLanguage)](#translateSheetAsync-java.lang.String-java.lang.String-com.aspose.gridjs.ITextTranslator-java.lang.String-) | Çalışma sayfasındaki tüm dize değerlerini hedef dile çevir. |
| [updateCell(String p, String uid)](#updateCell-java.lang.String-java.lang.String-) | Güncelleme işlemini uygular. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsWorkbook() {#GridJsWorkbook--}
```
public GridJsWorkbook()
```


GridJsWorkbook'ın yeni bir örneğini oluşturur.

### CacheImp {#CacheImp}
```
public static GridCacheForStream CacheImp
```


Önbellek depolama için özel uygulama, önbelleği akış şeklinde depolamak istiyorsanız, ayarlamanız ve uygulamanız gerekir.

### CalculateEngine {#CalculateEngine}
```
public static GridAbstractCalculationEngine CalculateEngine
```


Hesaplama motoru için özel uygulama, özel bir hesaplama yapmak istiyorsanız, onu ayarlamanız ve uygulamanız gerekir.

### PICTURE_TYPE {#PICTURE-TYPE}
```
public static final String PICTURE_TYPE
```


Görsel türü için sabit değer

### UpdateMonitor {#UpdateMonitor}
```
public static GridUpdateMonitor UpdateMonitor
```


Güncelleme işlemini izlemek için güncelleme izleyicisini alır/ayarlar

### burnRedactionFile(String excelFilePath, String uid) {#burnRedactionFile-java.lang.String-java.lang.String-}
```
public void burnRedactionFile(String excelFilePath, String uid)
```


Uygular (yanar) tüm kırpma işlemlerini, kırpma şekillerini ve hedef şekillerini kaldırarak veya hedef hücre aralığı içeriğini temizleyerek çalışma kitabında.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| excelFilePath | java.lang.String | Excel dosyasının dosya yolu. |
| uid | java.lang.String | Çalışma kitabı için benzersiz tanımlayıcı. Null veya boş ise, dosya yoluna göre yeni bir uid oluşturulur. |

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


\\u5a13\\u5474\\u6ace\\u93b5\\u20ac\\u93c8?JSON \\u7f02\\u64b3\\u74e8

### clearJsonCacheForUid(String uid) {#clearJsonCacheForUid-java.lang.String-}
```
public void clearJsonCacheForUid(String uid)
```


\\u93cd\\u89c4\\u5d41 uid \\u5a13\\u5474\\u6ace JSON \\u7f02\\u64b3\\u74e8\\u951b\\u5822\\u6564\\u6d5c?UpdateCell \\u7edb\\u590a\\u5f67\\u93c8?uid \\u9428\\u52eb\\u6e80\\u93c5\\ue224\\u7d1a

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |

### copyImageOrShape(String uid, String p) {#copyImageOrShape-java.lang.String-java.lang.String-}
```
public String copyImageOrShape(String uid, String p)
```


Görüntüyü veya şekli kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| p | java.lang.String | Hücre konumunu belirten işlem için JSON dizesi, çalışma sayfası adı, görüntü veya şekil için sol üst satır ve sol üst sütunu içerir\\u951b\\u5b94tc \{name:'sheet1',ri:1,ci:1,srcid:2,srcname:'sheet2',isshape:true\} |

**Returns:**
java.lang.String - Yeni kopyalanmış görüntünün JSON dizesi
### dispose() {#dispose--}
```
public void dispose()
```


Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür.

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
### errorJson(String msg) {#errorJson-java.lang.String-}
```
public String errorJson(String msg)
```


JSON formatında hata mesajı dizesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| msg | java.lang.String | Hata mesajı. |

**Returns:**
java.lang.String - JSON dizesi.
### exportToJson() {#exportToJson--}
```
public String exportToJson()
```


Bellek verisinden JSON dizesini alır, JSON içindeki varsayılan dosya adı: book1.

**Returns:**
java.lang.String - JSON dizesi.
### exportToJson(String filename) {#exportToJson-java.lang.String-}
```
public String exportToJson(String filename)
```


Bellek verisinden JSON dizesini alır, JSON içinde çıktı dosya adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya adı | java.lang.String | JSON içinde dosya adını belirtir. Null olarak ayarlanırsa, varsayılan dosya adı: book1.. |

**Returns:**
java.lang.String - JSON dizesi.
### exportToJsonStringBuilder(String filename) {#exportToJsonStringBuilder-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename)
```


Bellek verisinden JSON dizesini alır, JSON içinde çıktı dosya adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya adı | java.lang.String | JSON içinde dosya adını belirtir. Null olarak ayarlanırsa, varsayılan dosya adı: book1.. |

**Returns:**
java.lang.StringBuilder - JSON StringBuilder.
### exportToJsonStringBuilder(String filename, String uid) {#exportToJsonStringBuilder-java.lang.String-java.lang.String-}
```
public StringBuilder exportToJsonStringBuilder(String filename, String uid)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya adı | java.lang.String |  |
| uid | java.lang.String |  |

**Returns:**
java.lang.StringBuilder
### getCacheDirectory() {#getCacheDirectory--}
```
public String getCacheDirectory()
```


Elektronik tablo dosyasını depolamak için önbellek dizinini alır. Bu ayarlanmamışsa, [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) veya [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp) adresindeki statik özelliği kullanacağız.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getGridLoadFormat(String extension) {#getGridLoadFormat-java.lang.String-}
```
public static int getGridLoadFormat(String extension)
```


Dosya uzantısına göre yükleme biçimini alır

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| extension | java.lang.String | Dosya uzantısı, genellikle '.' ile başlar. |

**Returns:**
int - [GridLoadFormat](../../com.aspose.gridjs/gridloadformat).
### getImageStream(String uid, String picid, String cachedir) {#getImageStream-java.lang.String-java.lang.String-java.lang.String-}
```
public static InputStream getImageStream(String uid, String picid, String cachedir)
```


Resim akışını al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| picid | java.lang.String | Görsel kimliği. |
| cachedir | java.lang.String |  |

**Returns:**
java.io.InputStream - Görsel akışı
### getImageUrl(String uid, String picid, String delimiter) {#getImageUrl-java.lang.String-java.lang.String-java.lang.String-}
```
public static String getImageUrl(String uid, String picid, String delimiter)
```


Resim URL'sini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| picid | java.lang.String | Görsel kimliği. |
| delimiter | java.lang.String | Dize ayırıcı. |

**Returns:**
java.lang.String -
### getJsonByUid(String uid, String filename) {#getJsonByUid-java.lang.String-java.lang.String-}
```
public StringBuilder getJsonByUid(String uid, String filename)
```


Belirtilen benzersiz kimliği kullanarak önbellekten dosyanın JSON dizesini alır, JSON içinde çıktı dosya adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| dosya adı | java.lang.String | JSON içinde dosya adını belirtir. Null olarak ayarlanırsa, varsayılan dosya adı: book1. |

**Returns:**
java.lang.StringBuilder - JSON dizesi StringBuilder
### getOle(String uid, String sheetname, int oleid, String label) {#getOle-java.lang.String-java.lang.String-int-java.lang.String-}
```
public byte[] getOle(String uid, String sheetname, int oleid, String label)
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
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Çalışma kitabı ayarlarını temsil eder.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings)
### getSheetJsonWithCache(String uid, String sheetName, String fileName) {#getSheetJsonWithCache-java.lang.String-java.lang.String-java.lang.String-}
```
public String getSheetJsonWithCache(String uid, String sheetName, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93b8\\u56e7\\u757e sayfa \\u9428?JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |
| sheetName | java.lang.String | \\u5bb8\\u30e4\\u7d94\\u741b\\u3125\\u6095\\u7ec9?\* @param fileName \\u9358\\u71b7\\ue750\\u93c2\\u56e6\\u6b22\\u935a?\* @return JSON \\u701b\\u6943\\ue0c1\\u6d93? |
| fileName | java.lang.String |  |

**Returns:**
java.lang.String
### getUidForFile(String fileName) {#getUidForFile-java.lang.String-}
```
public static String getUidForFile(String fileName)
```


Verilen dosya adını kullanarak dosya önbelleği için yeni benzersiz bir kimlik oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Dosya adı. |

**Returns:**
java.lang.String -
### getWorkbookJsonWithCache(String uid, String fileName) {#getWorkbookJsonWithCache-java.lang.String-java.lang.String-}
```
public String getWorkbookJsonWithCache(String uid, String fileName)
```


\\u947e\\u5cf0\\u5f47\\u93c1\\u7fe0\\u91dc\\u5bb8\\u30e4\\u7d94\\u7ee8\\u8de8\\u6b91 JSON\\u951b\\u581d\\u752b\\u7f02\\u64b3\\u74e8\\u951b?\*

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | \\u93c2\\u56e6\\u6b22\\u9428\\u52eb\\u656e\\u6d93\\u20ac\\u93cd\\u56ea\\u7611 |
| fileName | java.lang.String | \\u9358\\u71b7\\ue750\\u93c2\\u56e6\\u6b22\\u935a?\* @return JSON \\u701b\\u6943\\ue0c1\\u6d93? |

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importExcelFile(InputStream filestream, int format) {#importExcelFile-java.io.InputStream-int-}
```
public void importExcelFile(InputStream filestream, int format)
```


Excel dosyasını dosya akışından yükleme biçimiyle içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filestream | java.io.InputStream | Excel dosyasının akışı . |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). Excel dosyasının LoadFormat'i. |

### importExcelFile(InputStream filestream, int format, String password) {#importExcelFile-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(InputStream filestream, int format, String password)
```


Excel dosyasını dosya akışından yükleme biçimi ve açma parolasıyla içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filestream | java.io.InputStream | Excel dosyasının akışı . |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). Excel dosyasının LoadFormat'i. |
| password | java.lang.String | Excel dosyasının açma şifresi. Değer null olabilir Eğer şifre ayarlanmamışsa. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


Excel dosyasını dosya yolundan içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Dosyanın tam yolu. |

### importExcelFile(String uid, InputStream filestream, int format) {#importExcelFile-java.lang.String-java.io.InputStream-int-}
```
public void importExcelFile(String uid, InputStream filestream, int format)
```


Excel dosyasını dosya akışından içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik, null olarak ayarlanırsa otomatik olarak oluşturulur. |
| filestream | java.io.InputStream | Excel dosyasının akışı . |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). Excel dosyasının LoadFormat'i. |

### importExcelFile(String uid, InputStream filestream, int format, String password) {#importExcelFile-java.lang.String-java.io.InputStream-int-java.lang.String-}
```
public void importExcelFile(String uid, InputStream filestream, int format, String password)
```


Excel dosyasını dosya akışından yükleme biçimi ve açma parolasıyla içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik, null olarak ayarlanırsa otomatik olarak oluşturulur. |
| filestream | java.io.InputStream | Excel dosyasının akışı . |
| format | int | [GridLoadFormat](../../com.aspose.gridjs/gridloadformat). Excel dosyasının LoadFormat'i. |
| password | java.lang.String | Excel dosyasının açma şifresi. Değer null olabilir Eğer şifre ayarlanmamışsa |

### importExcelFile(String uid, String fileName) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName)
```


Excel dosyasını dosya yolundan içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik, null olarak ayarlanırsa otomatik olarak oluşturulur. |
| fileName | java.lang.String | Dosyanın tam yolu. |

### importExcelFile(String uid, String fileName, String password) {#importExcelFile-java.lang.String-java.lang.String-java.lang.String-}
```
public void importExcelFile(String uid, String fileName, String password)
```


Excel dosyasını dosya yolundan ve açma parolasıyla içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik, null olarak ayarlanırsa otomatik olarak oluşturulur. |
| fileName | java.lang.String | Dosyanın tam yolu. |
| password | java.lang.String | Excel dosyasının açma şifresi. Değer null olabilir Eğer şifre ayarlanmamışsa. |

### importExcelFileFromJson(String json) {#importExcelFileFromJson-java.lang.String-}
```
public void importExcelFileFromJson(String json)
```


Excel dosyasını JSON formatındaki dizeden içe aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| json | java.lang.String | JSON format dizesi. |

### insertImage(String uid, String p, InputStream s, String imageUrl) {#insertImage-java.lang.String-java.lang.String-java.io.InputStream-java.lang.String-}
```
public String insertImage(String uid, String p, InputStream s, String imageUrl)
```


Çalışma sayfasına dosya akışından veya URL'den resim ekler (dosya akışı veya URL sağlanmalıdır) veya p.type, AutoShapeType'tan biri olduğunda şekil ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik |
| p | java.lang.String | Görüntü için hücre konumunu, çalışma sayfası adını, sol üst satırı, sol üst sütunu belirten işlemin JSON format dizesi\\u951b\\u5b94tc \{name:'sheet1',ri:1,ci:1\} |
| s | java.io.InputStream | Görüntü dosyasının dosya akışı |
| imageUrl | java.lang.String | Görüntü dosyasının URL'si |

**Returns:**
java.lang.String - Eklenen görüntünün JSON format dizesi
### jsonToStream(OutputStream stream, String filename) {#jsonToStream-java.io.OutputStream-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename)
```


In-memory Workbook'tan JSON oluştur ve belirtilen akışa yaz. İsteğe bağlı olarak oluşturulan JSON'ı daha hızlı sonraki erişim için önbelleğe al. JsonToStreamByUid ile temel farklar: - Bu yöntem mevcut in-memory Workbook durumunu (wb alanı) kullanır - JsonToStreamByUid Workbook'ı .cells önbellek dosyalarından diskte yeniden yükler - Bu yöntemi, değişikliklerden sonra mevcut workbook durumunu dışa aktarmak istediğinizde kullanın - Önceden önbelleğe alınmış bir dosya durumundan JSON'ı yeniden oluşturmanız gerektiğinde JsonToStreamByUid kullanın Önbellekleme davranışı (uid sağlandığında): - Oluşturma öncesi JSON önbelleğini kontrol eder (L1 bellek + L2 disk) - Önbellek yoksa, in-memory workbook'tan JSON oluşturur - Oluşturulan JSON gelecekteki istekler için önbellekte saklanır

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | JSON verilerini yazmak için çıktı akışı |
| dosya adı | java.lang.String | JSON içinde dosya adını belirtir. Null olarak ayarlanırsa, varsayılan dosya adı: book1. |

### jsonToStream(OutputStream stream, String filename, String uid) {#jsonToStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void jsonToStream(OutputStream stream, String filename, String uid)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| dosya adı | java.lang.String |  |
| uid | java.lang.String |  |

### jsonToStreamByUid(OutputStream stream, String uid, String filename) {#jsonToStreamByUid-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public boolean jsonToStreamByUid(OutputStream stream, String uid, String filename)
```


Belirtilen benzersiz kimliği kullanarak dosyanın JSON dizesini önbellekten alır, JSON içinde çıktı dosya adını ayarlar ve akışa yazar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Yazılacak akış |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| dosya adı | java.lang.String | JSON içinde dosya adını belirtir. Null olarak ayarlanırsa, varsayılan dosya adı: book1. |

**Returns:**
boolean
### lazyLoadingJson(String uid, String sheetName) {#lazyLoadingJson-java.lang.String-java.lang.String-}
```
public StringBuilder lazyLoadingJson(String uid, String sheetName)
```


Belirtilen benzersiz kimliği kullanarak dosyadaki belirtilen sayfanın JSON dizesini önbellekten alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| sheetName | java.lang.String | sayfa adı. |

**Returns:**
java.lang.StringBuilder - JSON dizesi StringBuilder
### lazyLoadingStream(OutputStream stream, String uid, String sheetName) {#lazyLoadingStream-java.io.OutputStream-java.lang.String-java.lang.String-}
```
public void lazyLoadingStream(OutputStream stream, String uid, String sheetName)
```


Belirtilen benzersiz kimliği kullanarak dosyadaki belirtilen sayfanın JSON dizesini önbellekten alır ve akışa yazar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Yazılacak akış |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| sheetName | java.lang.String | sayfa adı. |

### mergeExcelFileFromJson(String uid, String json) {#mergeExcelFileFromJson-java.lang.String-java.lang.String-}
```
public void mergeExcelFileFromJson(String uid, String json)
```


Bellek verisine toplu bir güncelleme uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| json | java.lang.String | Güncelleme JSON format dizesi. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr) {#redactFile-java.lang.String-java.lang.String-java.lang.String---}
```
public void redactFile(String excelFilePath, String uid, String[] arrayOfRedactionOpr)
```


JSON işlemleri dizisine dayanarak bir Excel dosyasında redaksiyon gerçekleştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| excelFilePath | java.lang.String | Kırpılacak Excel dosyasının dosya yolu. |
| uid | java.lang.String | Çalışma kitabı için benzersiz tanımlayıcı. Null veya boş ise, dosya yoluna göre yeni bir uid oluşturulur. |
| arrayOfRedactionOpr | java.lang.String[] | Uygulanacak kırpma işlemlerini temsil eden JSON dizesi dizisi. |

### saveToCacheWithFileName(String uid, String filename, String password) {#saveToCacheWithFileName-java.lang.String-java.lang.String-java.lang.String-}
```
public void saveToCacheWithFileName(String uid, String filename, String password)
```


Bellek verisini belirtilen dosya adıyla önbellek dosyasına kaydeder ve ayrıca açma parolasını ayarlar, kaydetme biçimi dosya adının uzantısına göre belirlenir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | java.lang.String | Dosya önbelleği için benzersiz kimlik. |
| dosya adı | java.lang.String | Kaydedilecek dosya adı. |
| password | java.lang.String | Excel dosyasının açma şifresi. Şifre ayarlanmamışsa değer null olabilir. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


Bellek verisini sream'e kaydeder, orijinal dosya biçimine göre belirlenir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Kaydedilecek akış. |

### saveToExcelFile(String path) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String path)
```


Bellek verisini dosya yoluna kaydeder, dosyanın uzantısı varsa kaydetme biçimi dosya uzantısına göre belirlenir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | java.lang.String | Kaydedilecek dosya yolu. |

### saveToHtml(OutputStream stream) {#saveToHtml-java.io.OutputStream-}
```
public void saveToHtml(OutputStream stream)
```


Bellek verisini sream'e kaydeder, kaydetme biçimi html'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Kaydedilecek akış. |

### saveToHtml(String path) {#saveToHtml-java.lang.String-}
```
public void saveToHtml(String path)
```


Bellek verisini dosya yoluna kaydeder, kaydetme biçimi html'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | java.lang.String | Kaydedilecek dosya yolu. |

### saveToPdf(OutputStream stream) {#saveToPdf-java.io.OutputStream-}
```
public void saveToPdf(OutputStream stream)
```


Bellek verisini sream'e kaydeder, kaydetme biçimi pdf'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Kaydedilecek akış. |

### saveToPdf(String path) {#saveToPdf-java.lang.String-}
```
public void saveToPdf(String path)
```


Bellek verilerini dosya yoluna kaydeder, kaydetme formatı pdf.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | java.lang.String | Kaydedilecek dosya yolu. |

### saveToXlsx(OutputStream stream) {#saveToXlsx-java.io.OutputStream-}
```
public void saveToXlsx(OutputStream stream)
```


Bellek verilerini akışa kaydeder, kaydetme formatı xlsx.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Kaydedilecek akış. |

### saveToXlsx(String path) {#saveToXlsx-java.lang.String-}
```
public void saveToXlsx(String path)
```


Bellek verilerini dosya yoluna kaydeder, kaydetme formatı xlsx.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | java.lang.String | Kaydedilecek dosya yolu. |

### setCacheDirectory(String value) {#setCacheDirectory-java.lang.String-}
```
public void setCacheDirectory(String value)
```


Elektronik tablo dosyasını depolamak için önbellek dizinini ayarlar. Bu ayarlanmamışsa, statik özelliği [Config.getFileCacheDirectory()](../../com.aspose.gridjs/config\#getFileCacheDirectory--) veya [CacheImp](../../com.aspose.gridjs/gridjsworkbook\#CacheImp) adresinden kullanacağız.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setImageUrlBase(String baseImageURL) {#setImageUrlBase-java.lang.String-}
```
public static void setImageUrlBase(String baseImageURL)
```


Denetleyiciden temel görüntü alma eylemi URL'sini ayarla.

**Remarks**

CacheImp null olduğunda, bunu ayarlamamız gerekir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| baseImageURL | java.lang.String | Temel görüntünün alma eylemi URL'si. |

### setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds) {#setInterruptMonitorForLoad-com.aspose.gridjs.GridInterruptMonitor-int-}
```
public void setInterruptMonitorForLoad(GridInterruptMonitor monitor, int calculateTimeoutMilliseconds)
```


Yükleme işlemi için InterruptMonitor'ı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | InterruptMonitor örneği. |
| calculateTimeoutMilliseconds | int | Dosya yükleme için milisaniye cinsinden zaman aşımı. |

### setInterruptMonitorForSave(GridInterruptMonitor monitor) {#setInterruptMonitorForSave-com.aspose.gridjs.GridInterruptMonitor-}
```
public void setInterruptMonitorForSave(GridInterruptMonitor monitor)
```


Kaydetme işlemi için InterruptMonitor'ı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| monitor | [GridInterruptMonitor](../../com.aspose.gridjs/gridinterruptmonitor) | InterruptMonitor örneği. |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridjs.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Çalışma kitabı ayarlarını temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridjs/gridworkbooksettings) |  |

### setTransParentView(String excelFilePath, String uid, boolean isTransparent) {#setTransParentView-java.lang.String-java.lang.String-boolean-}
```
public void setTransParentView(String excelFilePath, String uid, boolean isTransparent)
```


Çalışma kitabındaki redaksiyon şekillerinin saydamlığını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| excelFilePath | java.lang.String | Excel dosyasının dosya yolu. |
| uid | java.lang.String | Çalışma kitabı için benzersiz tanımlayıcı. Null veya boş ise, dosya yoluna göre yeni bir uid oluşturulur. |
| isTransparent | boolean | Doğru ise, şeffaflığı 0.89 (yarı şeffaf) olarak ayarlar; yanlış ise, şeffaflığı 1 (tamamen opak/görünmez) olarak ayarlar. |

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
java.lang.String - Güncelleme sonucunun JSON formatındaki dizesi.
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


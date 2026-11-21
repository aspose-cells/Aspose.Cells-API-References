---
title: "Yapılandırma"
second_title: "Aspose.Cells for Java API Referansı"
description: "GridJs için tüm statik ayarları temsil eder"
type: docs
url: /tr/java/com.aspose.gridjs/config/
---

**Inheritance:**
java.lang.Object
```
public class Config
```

GridJs için tüm statik ayarları temsil eder
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Config()](#Config--) |  |
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [RedactionUseClientGenerateId](#RedactionUseClientGenerateId) | Kırpma ile ilgili işlemlerde gerçek şekil kimliği yerine istemci tarafından oluşturulan kimliğin kullanılıp kullanılmayacağını gösterir |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitColumnsOnLoad()](#getAutoFitColumnsOnLoad--) | Dosya yüklenirken sütun genişliklerinin otomatik olarak ayarlanıp ayarlanmayacağını gösterir. |
| [getAutoFitRowsHeightOnLoad()](#getAutoFitRowsHeightOnLoad--) | Dosya yüklenirken satır yüksekliğinin otomatik olarak ayarlanıp ayarlanmayacağını belirtir. |
| [getAutoOptimizeForLargeCells()](#getAutoOptimizeForLargeCells--) | Büyük hücreli çalışma sayfası için yük performansının otomatik olarak optimize edilip edilmediğini alır. |
| [getBaseRouteName()](#getBaseRouteName--) | GridJs denetleyici URL'si için temel rota adını alır. Varsayılan "/GridJs2" dır. |
| [getClass()](#getClass--) |  |
| [getEmptySheetMaxCol()](#getEmptySheetMaxCol--) | Boş bir çalışma sayfası için varsayılan maksimum sütunu alır. |
| [getEmptySheetMaxRow()](#getEmptySheetMaxRow--) | Boş bir çalışma sayfası için varsayılan maksimum satırı alır. |
| [getEnableChartClientRendering()](#getEnableChartClientRendering--) | İstemci tarafı grafik render'ının etkinleştirilip etkinleştirilmeyeceğini alır. |
| [getFileCacheDirectory()](#getFileCacheDirectory--) | Elektronik tablo dosyasını depolamak için önbellek dizinini alır. |
| [getIgnoreEmptyContent()](#getIgnoreEmptyContent--) | Veri, stil, birleştirilmiş hücreler ve şekilleri içeren maksimum aralığın gösterilip gösterilmeyeceğini alır. |
| [getIslimitShapeOrImage()](#getIslimitShapeOrImage--) | Bir çalışma sayfasında toplam görüntülenen şekil/görüntü sayısının sınırlanıp sınırlanmayacağını alır, true olarak ayarlanırsa, GridJs bir çalışma sayfasındaki görüntülenen şekil veya görüntülerin toplam sayısını MaxShapeOrImageCount değerine sınırlar, varsayılan değer true'tır. |
| [getJsonCache()](#getJsonCache--) | JSON önbellek yapılandırma seçeneklerini alır. |
| [getLazyLoading()](#getLazyLoading--) | Yalnızca etkin çalışma sayfasının yüklenip yüklenmeyeceğini alır, varsayılan değer false'tur. |
| [getMaxPdfSaveSeconds()](#getMaxPdfSaveSeconds--) | PDF'ye kaydedilirken maksimum zaman aşımı saniyesini alır. |
| [getMaxShapeOrImageCount()](#getMaxShapeOrImageCount--) | Etkin sayfadaki görüntülenen şekil veya görüntülerin toplam sayısını alır, IslimitShapeOrImage=true olduğunda etkili olur. |
| [getMaxShapeOrImageWidthOrHeight()](#getMaxShapeOrImageWidthOrHeight--) | Bir şekil veya görüntü için maksimum genişlik veya yüksekliği alır, GridJs bu değerden daha büyük genişlik veya yüksekliğe sahip şekil veya görüntüyü yok sayar, IslimitShapeOrImage=true olduğunda etkili olur. |
| [getMaxTotalShapeOrImageCount()](#getMaxTotalShapeOrImageCount--) | Çalışma kitabındaki görüntülenen şekil veya görüntülerin toplam sayısını alır, IslimitShapeOrImage=true olduğunda etkili olur. |
| [getMessageTopic()](#getMessageTopic--) | Websocket hedeflerini "\/topic" önekiyle alır. Varsayılan değer "\/topic/opr"'dir. Yalnızca işbirlikçi modda kullanılır. |
| [getPictureCacheDirectory()](#getPictureCacheDirectory--) | Resimler için önbellek dizinini alır. |
| [getSameImageDetecting()](#getSameImageDetecting--) | Resimlerin aynı kaynağa sahip olup olmadığını kontrol edip etmeyeceğini alır, varsayılan değer true'tır. |
| [getSaveHtmlAsZip()](#getSaveHtmlAsZip--) | HTML dosyasını zip arşivi olarak kaydedip kaydetmeyeceğini alır, varsayılan değer false'tur. |
| [getShowChartSheet()](#getShowChartSheet--) | Grafik çalışma sayfasının gösterilip gösterilmeyeceğini alır. |
| [getSkipInvisibleShapes()](#getSkipInvisibleShapes--) | UI'da görünmez olan şekilleri atlayıp atlamayacağını alır, varsayılan değer true. |
| [getUsePrintArea()](#getUsePrintArea--) | Çalışma sayfası PrintArea ayarına sahip olduğunda UI görüntü aralığı için PageSetup.PrintArea kullanılacağını alır. |
| [hashCode()](#hashCode--) |  |
| [isCollaborative()](#isCollaborative--) | Ortak düzenlemeyi destekleyip desteklemeyeceğini alır, varsayılan değer false. |
| [isWasm()](#isWasm--) | GridJs'in bir sunucu süreci yerine tarayıcı WebAssembly ana bilgisayarında çalışıp çalışmadığını alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitColumnsOnLoad(boolean value)](#setAutoFitColumnsOnLoad-boolean-) | Dosya yüklenirken sütun genişliklerinin otomatik olarak ayarlanıp ayarlanmayacağını gösterir. |
| [setAutoFitRowsHeightOnLoad(boolean value)](#setAutoFitRowsHeightOnLoad-boolean-) | Dosya yüklenirken satır yüksekliğinin otomatik olarak ayarlanıp ayarlanmayacağını belirtir. |
| [setAutoOptimizeForLargeCells(boolean value)](#setAutoOptimizeForLargeCells-boolean-) | Büyük hücreli çalışma sayfası için yük performansını otomatik olarak optimize edip etmeyeceğini ayarlar. |
| [setBaseRouteName(String value)](#setBaseRouteName-java.lang.String-) | GridJs denetleyici URL'si için temel rota adını ayarlar. Varsayılan "/GridJs2" dır. |
| [setCollaborative(boolean value)](#setCollaborative-boolean-) | Ortak düzenlemeyi destekleyip desteklemeyeceğini ayarlar, varsayılan değer false. |
| [setEmptySheetMaxCol(int value)](#setEmptySheetMaxCol-int-) | Boş bir çalışma sayfası için varsayılan maksimum sütunu ayarlar. |
| [setEmptySheetMaxRow(int value)](#setEmptySheetMaxRow-int-) | Boş bir çalışma sayfası için varsayılan maksimum satırı ayarlar. |
| [setEnableChartClientRendering(boolean value)](#setEnableChartClientRendering-boolean-) | İstemci tarafı grafik render'ını etkinleştirip etkinleştirmeyeceğini ayarlar. |
| [setFileCacheDirectory(String value)](#setFileCacheDirectory-java.lang.String-) | Elektronik tablo dosyasını depolamak için önbellek dizinini ayarlar. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Yazı tipi klasörünü ayarlar |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Yazı tipleri klasörlerini ayarlar |
| [setIgnoreEmptyContent(boolean value)](#setIgnoreEmptyContent-boolean-) | Veri, stil, birleştirilmiş hücreler ve şekilleri içeren maksimum aralığı gösterip göstermeyeceğini ayarlar. |
| [setIslimitShapeOrImage(boolean value)](#setIslimitShapeOrImage-boolean-) | Bir çalışma sayfasındaki toplam görüntülenen şekil/görsel sayısını sınırlayıp sınırlamayacağını ayarlar, true olarak ayarlanırsa GridJs, bir çalışma sayfasındaki görüntülenen şekil veya görsel sayısını MaxShapeOrImageCount değerine sınırlar, varsayılan değer true. |
| [setJsonCache(JsonCacheOptions value)](#setJsonCache-com.aspose.gridjs.JsonCacheOptions-) | JSON önbellek yapılandırma seçeneklerini ayarlar. |
| [setLazyLoading(boolean value)](#setLazyLoading-boolean-) | Yalnızca aktif çalışma sayfasını yükleyip yüklemeyeceğini ayarlar, varsayılan değer false. |
| [setMaxPdfSaveSeconds(int value)](#setMaxPdfSaveSeconds-int-) | PDF'ye kaydederken maksimum zaman aşımı saniyesini ayarlar. |
| [setMaxShapeOrImageCount(int value)](#setMaxShapeOrImageCount-int-) | Aktif sayfadaki görüntülenen şekil veya görsel toplam sayısını ayarlar, IslimitShapeOrImage=true olduğunda etkili olur. |
| [setMaxShapeOrImageWidthOrHeight(int value)](#setMaxShapeOrImageWidthOrHeight-int-) | Bir şekil veya görsel için maksimum genişlik veya yüksekliği ayarlar, GridJs bu değerden daha geniş veya yüksek olan şekil veya görselleri yok sayar, IslimitShapeOrImage=true olduğunda etkili olur. |
| [setMaxTotalShapeOrImageCount(int value)](#setMaxTotalShapeOrImageCount-int-) | Çalışma kitabındaki görüntülenen şekil veya görsel toplam sayısını ayarlar, IslimitShapeOrImage=true olduğunda etkili olur. |
| [setMessageTopic(String value)](#setMessageTopic-java.lang.String-) | Websocket hedeflerini "/topic" önekiyle ayarlar. Varsayılan değer "/topic/opr". Yalnızca ortak çalışma modunda kullanılır. |
| [setPictureCacheDirectory(String value)](#setPictureCacheDirectory-java.lang.String-) | Resimler için önbellek dizinini ayarlar. |
| [setSameImageDetecting(boolean value)](#setSameImageDetecting-boolean-) | Resimlerin aynı kaynağa sahip olup olmadığını kontrol edip etmeyeceğini ayarlar, varsayılan değer true. |
| [setSaveHtmlAsZip(boolean value)](#setSaveHtmlAsZip-boolean-) | HTML dosyasını zip arşivi olarak kaydedip kaydetmeyeceğini ayarlar, varsayılan değer false. |
| [setShowChartSheet(boolean value)](#setShowChartSheet-boolean-) | Grafik çalışma sayfasını gösterip göstermeyeceğini ayarlar. |
| [setSkipInvisibleShapes(boolean value)](#setSkipInvisibleShapes-boolean-) | UI için görünmez olan şekilleri atlayıp atlamayacağını ayarlar, varsayılan değer true'dur. |
| [setUsePrintArea(boolean value)](#setUsePrintArea-boolean-) | Çalışma sayfası PrintArea ayarına sahip olduğunda UI görüntü aralığı için PageSetup.PrintArea kullanımını ayarlar. |
| [setWasm(boolean value)](#setWasm-boolean-) | GridJs'in bir sunucu süreci yerine tarayıcı WebAssembly ana bilgisayarında çalışıp çalışmayacağını ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Config() {#Config--}
```
public Config()
```


### RedactionUseClientGenerateId {#RedactionUseClientGenerateId}
```
public static boolean RedactionUseClientGenerateId
```


Kırpma ile ilgili işlemlerde gerçek şekil kimliği yerine istemci tarafından oluşturulan kimliğin kullanılıp kullanılmayacağını gösterir

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
### getAutoFitColumnsOnLoad() {#getAutoFitColumnsOnLoad--}
```
public static boolean getAutoFitColumnsOnLoad()
```


Dosya yüklenirken sütun genişliklerinin otomatik olarak ayarlanıp ayarlanmayacağını belirtir. Varsayılan değer `false` dır. Uyarı: Bunu `true` olarak ayarlamak, yükleme sonrasında tüm sütunların otomatik ayarlanmasını gerçekleştirir ve bu, performans üzerinde fark edilir bir etki yaratabilir.

**Returns:**
boolean
### getAutoFitRowsHeightOnLoad() {#getAutoFitRowsHeightOnLoad--}
```
public static boolean getAutoFitRowsHeightOnLoad()
```


Dosya yüklenirken satır yüksekliğinin otomatik olarak ayarlanıp ayarlanmayacağını belirtir. Varsayılan değer `false` dır. Uyarı: Bunu `true` olarak ayarlamak, yükleme sonrasında tüm satırların otomatik ayarlanmasını gerçekleştirir ve bu, performans üzerinde fark edilir bir etki yaratabilir.

**Returns:**
boolean
### getAutoOptimizeForLargeCells() {#getAutoOptimizeForLargeCells--}
```
public static boolean getAutoOptimizeForLargeCells()
```


Büyük hücreli çalışma sayfası için yük performansını otomatik olarak optimize edip etmeyeceğini alır. Yük süresini azaltmak için bazı stil /kenarları yok sayar. Varsayılan değer true'tir.

**Returns:**
boolean
### getBaseRouteName() {#getBaseRouteName--}
```
public static String getBaseRouteName()
```


GridJs denetleyici URL'si için temel rota adını alır. Varsayılan "/GridJs2" dır.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEmptySheetMaxCol() {#getEmptySheetMaxCol--}
```
public static int getEmptySheetMaxCol()
```


Boş bir çalışma sayfası için varsayılan maksimum sütunu alır. Varsayılan değer 15'tir.

**Returns:**
int
### getEmptySheetMaxRow() {#getEmptySheetMaxRow--}
```
public static int getEmptySheetMaxRow()
```


Boş bir çalışma sayfası için varsayılan maksimum satırı alır. Varsayılan değer 12'dir.

**Returns:**
int
### getEnableChartClientRendering() {#getEnableChartClientRendering--}
```
public static boolean getEnableChartClientRendering()
```


İstemci tarafı grafik render'ını etkinleştirip etkinleştirilmeyeceğini alır. False olarak ayarlanırsa, GridJs yalnızca sunucu tarafından oluşturulan grafik görüntüleri/şekilleri kullanır. Varsayılan değer true dır.

**Returns:**
boolean
### getFileCacheDirectory() {#getFileCacheDirectory--}
```
public static String getFileCacheDirectory()
```


Elektronik tablo dosyasını depolamak için önbellek dizinini alır. GridJs'i kullanmadan önce bunu belirli bir yola ayarlamamız gerekir.

**Returns:**
java.lang.String
### getIgnoreEmptyContent() {#getIgnoreEmptyContent--}
```
public static boolean getIgnoreEmptyContent()
```


Veri, stil, birleştirilmiş hücreler ve şekilleri içeren maksimum aralığın gösterilip gösterilmeyeceğini alır. Son satır veya sütun değer ve formül içermeyen ancak özel stil olan hücreler içeriyorsa, bu değer true olduğunda o satır/sütun gösterilmez\u9286?\* Varsayılan değer true'tir.

**Returns:**
boolean
### getIslimitShapeOrImage() {#getIslimitShapeOrImage--}
```
public static boolean getIslimitShapeOrImage()
```


Bir çalışma sayfasında toplam görüntülenen şekil/görüntü sayısının sınırlanıp sınırlanmayacağını alır, true olarak ayarlanırsa, GridJs bir çalışma sayfasındaki görüntülenen şekil veya görüntülerin toplam sayısını MaxShapeOrImageCount değerine sınırlar, varsayılan değer true'tır.

**Returns:**
boolean
### getJsonCache() {#getJsonCache--}
```
public static JsonCacheOptions getJsonCache()
```


JSON önbellek yapılandırma seçeneklerini alır. Oluşturulan çalışma kitabı JSON'ı için bellek (L1) ve disk (L2) önbellek davranışını kontrol eder.

**Returns:**
[JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions)
### getLazyLoading() {#getLazyLoading--}
```
public static boolean getLazyLoading()
```


Yalnızca etkin çalışma sayfasının yüklenip yüklenmeyeceğini alır, varsayılan değer false'tur.

**Returns:**
boolean
### getMaxPdfSaveSeconds() {#getMaxPdfSaveSeconds--}
```
public static int getMaxPdfSaveSeconds()
```


PDF'ye kaydederken maksimum zaman aşımı saniyesini alır. Varsayılan değer 10'dur.

**Returns:**
int
### getMaxShapeOrImageCount() {#getMaxShapeOrImageCount--}
```
public static int getMaxShapeOrImageCount()
```


Etkin sayfadaki görüntülenen şekil veya resimlerin toplam sayısını alır, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 100'dür.

**Returns:**
int
### getMaxShapeOrImageWidthOrHeight() {#getMaxShapeOrImageWidthOrHeight--}
```
public static int getMaxShapeOrImageWidthOrHeight()
```


Bir şekil veya resim için maksimum genişlik veya yüksekliği alır, GridJs bu değerden daha büyük genişlik veya yüksekliğe sahip şekil veya resmi yok sayar, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 10000'dir.

**Returns:**
int
### getMaxTotalShapeOrImageCount() {#getMaxTotalShapeOrImageCount--}
```
public static int getMaxTotalShapeOrImageCount()
```


Çalışma kitabındaki görüntülenen şekil veya resimlerin toplam sayısını alır, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 300'dür.

**Returns:**
int
### getMessageTopic() {#getMessageTopic--}
```
public static String getMessageTopic()
```


Websocket hedeflerini "\/topic" önekiyle alır. Varsayılan değer "\/topic/opr"'dir. Yalnızca işbirlikçi modda kullanılır.

**Returns:**
java.lang.String
### getPictureCacheDirectory() {#getPictureCacheDirectory--}
```
public static String getPictureCacheDirectory()
```


Resimler için önbellek dizinini alır.(bu, GridJsWorkbook.CacheImp null olduğunda etkili olur) Varsayılan yol, FileCacheDirectory içinde "\_piccache" olacaktır.

**Returns:**
java.lang.String
### getSameImageDetecting() {#getSameImageDetecting--}
```
public static boolean getSameImageDetecting()
```


Resimlerin aynı kaynağa sahip olup olmadığını kontrol edip etmeyeceğini alır, varsayılan değer true'tır.

**Returns:**
boolean
### getSaveHtmlAsZip() {#getSaveHtmlAsZip--}
```
public static boolean getSaveHtmlAsZip()
```


HTML dosyasını zip arşivi olarak kaydedip kaydetmeyeceğini alır, varsayılan değer false'tur.

**Returns:**
boolean
### getShowChartSheet() {#getShowChartSheet--}
```
public static boolean getShowChartSheet()
```


Grafik çalışma sayfasının gösterilip gösterilmeyeceğini alır. Varsayılan değer false'tur.

**Returns:**
boolean
### getSkipInvisibleShapes() {#getSkipInvisibleShapes--}
```
public static boolean getSkipInvisibleShapes()
```


UI'da görünmez olan şekilleri atlayıp atlamayacağını alır, varsayılan değer true.

**Returns:**
boolean
### getUsePrintArea() {#getUsePrintArea--}
```
public static boolean getUsePrintArea()
```


Çalışma sayfası PrintArea ayarına sahip olduğunda UI görüntü aralığı için PageSetup.PrintArea kullanımını alır. Varsayılan değer false'tur.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollaborative() {#isCollaborative--}
```
public static boolean isCollaborative()
```


Ortak düzenlemeyi destekleyip desteklemeyeceğini alır, varsayılan değer false.

**Returns:**
boolean
### isWasm() {#isWasm--}
```
public static boolean isWasm()
```


GridJs'in bir sunucu süreci yerine tarayıcı WebAssembly hostu içinde çalışıp çalışmadığını alır. True olduğunda, FileCacheDirectory / disk / interrupt-thread yolu kullanılmaz ve dosya önbelleği GridJsOptions.CacheImp üzerinden gelmelidir. GridJsOptions.IsWasm, GridJs hizmeti oluşturulduğunda bunu ayarlar, böylece tek bir Aspose.Cells.GridJs.dll her iki hostu da hizmet verir. Varsayılan değer false dır.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoFitColumnsOnLoad(boolean value) {#setAutoFitColumnsOnLoad-boolean-}
```
public static void setAutoFitColumnsOnLoad(boolean value)
```


Dosya yüklenirken sütun genişliklerinin otomatik olarak ayarlanıp ayarlanmayacağını belirtir. Varsayılan değer `false` dır. Uyarı: Bunu `true` olarak ayarlamak, yükleme sonrasında tüm sütunların otomatik ayarlanmasını gerçekleştirir ve bu, performans üzerinde fark edilir bir etki yaratabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoFitRowsHeightOnLoad(boolean value) {#setAutoFitRowsHeightOnLoad-boolean-}
```
public static void setAutoFitRowsHeightOnLoad(boolean value)
```


Dosya yüklenirken satır yüksekliğinin otomatik olarak ayarlanıp ayarlanmayacağını belirtir. Varsayılan değer `false` dır. Uyarı: Bunu `true` olarak ayarlamak, yükleme sonrasında tüm satırların otomatik ayarlanmasını gerçekleştirir ve bu, performans üzerinde fark edilir bir etki yaratabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoOptimizeForLargeCells(boolean value) {#setAutoOptimizeForLargeCells-boolean-}
```
public static void setAutoOptimizeForLargeCells(boolean value)
```


Büyük hücreli çalışma sayfası için yük performansını otomatik olarak optimize edip etmeyeceğini ayarlar. Yük süresini azaltmak için bazı stil /kenarları yok sayar. Varsayılan değer true'tir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBaseRouteName(String value) {#setBaseRouteName-java.lang.String-}
```
public static void setBaseRouteName(String value)
```


GridJs denetleyici URL'si için temel rota adını ayarlar. Varsayılan "/GridJs2" dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCollaborative(boolean value) {#setCollaborative-boolean-}
```
public static void setCollaborative(boolean value)
```


Ortak düzenlemeyi destekleyip desteklemeyeceğini ayarlar, varsayılan değer false.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEmptySheetMaxCol(int value) {#setEmptySheetMaxCol-int-}
```
public static void setEmptySheetMaxCol(int value)
```


Boş bir çalışma sayfası için varsayılan maksimum sütunu ayarlar. Varsayılan değer 15'tir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setEmptySheetMaxRow(int value) {#setEmptySheetMaxRow-int-}
```
public static void setEmptySheetMaxRow(int value)
```


Boş bir çalışma sayfası için varsayılan maksimum satırı ayarlar. Varsayılan değer 12'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setEnableChartClientRendering(boolean value) {#setEnableChartClientRendering-boolean-}
```
public static void setEnableChartClientRendering(boolean value)
```


İstemci tarafı grafik render'ını etkinleştirip etkinleştirilmeyeceğini ayarlar. False olarak ayarlanırsa, GridJs yalnızca sunucu tarafından oluşturulan grafik görüntüleri/şekilleri kullanır. Varsayılan değer true dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFileCacheDirectory(String value) {#setFileCacheDirectory-java.lang.String-}
```
public static void setFileCacheDirectory(String value)
```


Elektronik tablo dosyasını depolamak için önbellek dizinini ayarlar. GridJs'i kullanmadan önce bunu belirli bir yola ayarlamamız gerekir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Yazı tipi klasörünü ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontFolder | java.lang.String | TrueType yazı tiplerini içeren klasör. |
| recursive | boolean | Alt klasörlerin taranıp taranmayacağını belirler. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Yazı tipleri klasörlerini ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontFolders | java.lang.String[] | TrueType yazı tiplerini içeren klasörler. |
| recursive | boolean | Alt klasörlerin taranıp taranmayacağını belirler. |

### setIgnoreEmptyContent(boolean value) {#setIgnoreEmptyContent-boolean-}
```
public static void setIgnoreEmptyContent(boolean value)
```


Veri, stil, birleştirilmiş hücreler ve şekilleri içeren maksimum aralığın gösterilip gösterilmeyeceğini ayarlar. Son satır veya sütun değer ve formül içermeyen ancak özel stil olan hücreler içeriyorsa, bu değer true olduğunda o satır/sütun gösterilmez\u9286?\* Varsayılan değer true'tir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setIslimitShapeOrImage(boolean value) {#setIslimitShapeOrImage-boolean-}
```
public static void setIslimitShapeOrImage(boolean value)
```


Bir çalışma sayfasındaki toplam görüntülenen şekil/görsel sayısını sınırlayıp sınırlamayacağını ayarlar, true olarak ayarlanırsa GridJs, bir çalışma sayfasındaki görüntülenen şekil veya görsel sayısını MaxShapeOrImageCount değerine sınırlar, varsayılan değer true.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setJsonCache(JsonCacheOptions value) {#setJsonCache-com.aspose.gridjs.JsonCacheOptions-}
```
public static void setJsonCache(JsonCacheOptions value)
```


JSON önbellek yapılandırma seçeneklerini ayarlar. Oluşturulan çalışma kitabı JSON'ı için hem bellek (L1) hem de disk (L2) önbellek davranışını kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions) |  |

### setLazyLoading(boolean value) {#setLazyLoading-boolean-}
```
public static void setLazyLoading(boolean value)
```


Yalnızca aktif çalışma sayfasını yükleyip yüklemeyeceğini ayarlar, varsayılan değer false.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMaxPdfSaveSeconds(int value) {#setMaxPdfSaveSeconds-int-}
```
public static void setMaxPdfSaveSeconds(int value)
```


PDF'ye kaydedilirken maksimum zaman aşımı saniyesini ayarlar. Varsayılan değer 10'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMaxShapeOrImageCount(int value) {#setMaxShapeOrImageCount-int-}
```
public static void setMaxShapeOrImageCount(int value)
```


Etkin sayfadaki görüntülenen şekil veya resimlerin toplam sayısını ayarlar, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 100'dür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMaxShapeOrImageWidthOrHeight(int value) {#setMaxShapeOrImageWidthOrHeight-int-}
```
public static void setMaxShapeOrImageWidthOrHeight(int value)
```


Bir şekil veya resim için maksimum genişlik veya yüksekliği ayarlar, GridJs bu genişlik veya yüksekliği aşan şekil veya resmi yok sayar, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 10000'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMaxTotalShapeOrImageCount(int value) {#setMaxTotalShapeOrImageCount-int-}
```
public static void setMaxTotalShapeOrImageCount(int value)
```


Çalışma kitabındaki görüntülenen şekil veya resimlerin toplam sayısını ayarlar, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 300'dür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMessageTopic(String value) {#setMessageTopic-java.lang.String-}
```
public static void setMessageTopic(String value)
```


Websocket hedeflerini "/topic" önekiyle ayarlar. Varsayılan değer "/topic/opr". Yalnızca ortak çalışma modunda kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPictureCacheDirectory(String value) {#setPictureCacheDirectory-java.lang.String-}
```
public static void setPictureCacheDirectory(String value)
```


Resimler için önbellek dizinini ayarlar. (Bu, GridJsWorkbook.CacheImp null olduğunda etkili olur) Varsayılan yol, FileCacheDirectory içinde "\_piccache" olacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setSameImageDetecting(boolean value) {#setSameImageDetecting-boolean-}
```
public static void setSameImageDetecting(boolean value)
```


Resimlerin aynı kaynağa sahip olup olmadığını kontrol edip etmeyeceğini ayarlar, varsayılan değer true.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSaveHtmlAsZip(boolean value) {#setSaveHtmlAsZip-boolean-}
```
public static void setSaveHtmlAsZip(boolean value)
```


HTML dosyasını zip arşivi olarak kaydedip kaydetmeyeceğini ayarlar, varsayılan değer false.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowChartSheet(boolean value) {#setShowChartSheet-boolean-}
```
public static void setShowChartSheet(boolean value)
```


Grafik çalışma sayfasının gösterilip gösterilmeyeceğini ayarlar. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSkipInvisibleShapes(boolean value) {#setSkipInvisibleShapes-boolean-}
```
public static void setSkipInvisibleShapes(boolean value)
```


UI için görünmez olan şekilleri atlayıp atlamayacağını ayarlar, varsayılan değer true'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setUsePrintArea(boolean value) {#setUsePrintArea-boolean-}
```
public static void setUsePrintArea(boolean value)
```


Çalışma sayfasının PrintArea için PageSetup ayarı olduğunda UI görüntüleme aralığı için PageSetup.PrintArea kullanılmasını ayarlar. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setWasm(boolean value) {#setWasm-boolean-}
```
public static void setWasm(boolean value)
```


GridJs'in bir sunucu süreci yerine tarayıcı WebAssembly hostu içinde çalışıp çalışmayacağını ayarlar. True olduğunda, FileCacheDirectory / disk / interrupt-thread yolu kullanılmaz ve dosya önbelleği GridJsOptions.CacheImp üzerinden gelmelidir. GridJsOptions.IsWasm, GridJs hizmeti oluşturulduğunda bunu ayarlar, böylece tek bir Aspose.Cells.GridJs.dll her iki hostu da hizmet verir. Varsayılan değer false dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### toString() {#toString--}
```
public String toString()
```




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


---
title: "GridJsOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "GridJs için tüm yükleme seçeneklerini temsil eder"
type: docs
url: /tr/java/com.aspose.gridjs/gridjsoptions/
---

**Inheritance:**
java.lang.Object
```
public class GridJsOptions
```

GridJs için tüm yükleme seçeneklerini temsil eder
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GridJsOptions()](#GridJsOptions--) |  |
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [CacheImp](#CacheImp) | Önbellek depolama için özel uygulama, önbelleği akış şeklinde depolamak istiyorsanız, ayarlamanız ve uygulamanız gerekir. |
| [RedactionUseClientGenerateId](#RedactionUseClientGenerateId) | Kırpma ile ilgili işlemlerde gerçek şekil kimliği yerine istemci tarafından oluşturulan kimliğin kullanılıp kullanılmayacağını gösterir |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitColumnsOnLoad()](#getAutoFitColumnsOnLoad--) | Dosya yüklenirken sütun genişliklerinin otomatik ayarlanıp ayarlanmayacağını gösterir, varsayılan değer false'tur. |
| [getAutoFitRowsHeightOnLoad()](#getAutoFitRowsHeightOnLoad--) | Dosya yüklenirken satır yüksekliğinin otomatik ayarlanıp ayarlanmayacağını gösterir, varsayılan değer false'tur. |
| [getAutoOptimizeForLargeCells()](#getAutoOptimizeForLargeCells--) | Büyük hücreli çalışma sayfası için yük performansının otomatik olarak optimize edilip edilmediğini alır. |
| [getBaseRouteName()](#getBaseRouteName--) | GridJs denetleyicisi için rota URL temel adını alır. Varsayılan değer GridJs2'dir. |
| [getClass()](#getClass--) |  |
| [getEmptySheetMaxCol()](#getEmptySheetMaxCol--) | Boş bir çalışma sayfası için varsayılan maksimum sütunu alır. |
| [getEmptySheetMaxRow()](#getEmptySheetMaxRow--) | Boş bir çalışma sayfası için varsayılan maksimum satırı alır. |
| [getEnableChartClientRendering()](#getEnableChartClientRendering--) | İstemci tarafı grafik render'ının etkinleştirilip etkinleştirilmeyeceğini alır. |
| [getFileCacheDirectory()](#getFileCacheDirectory--) | Elektronik tablo dosyasını depolamak için önbellek dizinini alır. |
| [getFontFolders()](#getFontFolders--) | Render edilen resim/şekillerdeki yazı tipleri için yazı tipi klasörlerini alır. |
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
| [setAutoFitColumnsOnLoad(boolean value)](#setAutoFitColumnsOnLoad-boolean-) | Dosya yüklenirken sütun genişliklerinin otomatik ayarlanıp ayarlanmayacağını gösterir, varsayılan değer false'tur. |
| [setAutoFitRowsHeightOnLoad(boolean value)](#setAutoFitRowsHeightOnLoad-boolean-) | Dosya yüklenirken satır yüksekliğinin otomatik ayarlanıp ayarlanmayacağını gösterir, varsayılan değer false'tur. |
| [setAutoOptimizeForLargeCells(boolean value)](#setAutoOptimizeForLargeCells-boolean-) | Büyük hücreli çalışma sayfası için yük performansını otomatik olarak optimize edip etmeyeceğini ayarlar. |
| [setBaseRouteName(String value)](#setBaseRouteName-java.lang.String-) | GridJs denetleyicisi için rota URL temel adını ayarlar, varsayılan değer GridJs2. |
| [setCollaborative(boolean value)](#setCollaborative-boolean-) | Ortak düzenlemeyi destekleyip desteklemeyeceğini ayarlar, varsayılan değer false. |
| [setEmptySheetMaxCol(int value)](#setEmptySheetMaxCol-int-) | Boş bir çalışma sayfası için varsayılan maksimum sütunu ayarlar. |
| [setEmptySheetMaxRow(int value)](#setEmptySheetMaxRow-int-) | Boş bir çalışma sayfası için varsayılan maksimum satırı ayarlar. |
| [setEnableChartClientRendering(boolean value)](#setEnableChartClientRendering-boolean-) | İstemci tarafı grafik render'ını etkinleştirip etkinleştirmeyeceğini ayarlar. |
| [setFileCacheDirectory(String value)](#setFileCacheDirectory-java.lang.String-) | Elektronik tablo dosyasını depolamak için önbellek dizinini ayarlar. |
| [setFontFolders(String[] value)](#setFontFolders-java.lang.String---) | Render edilmiş resim/şekillerdeki yazı tipleri için yazı tipi klasörlerini ayarlar. |
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
### GridJsOptions() {#GridJsOptions--}
```
public GridJsOptions()
```


### CacheImp {#CacheImp}
```
public GridCacheForStream CacheImp
```


Önbellek depolama için özel uygulama, önbelleği akış şeklinde depolamak istiyorsanız, bunu ayarlamanız ve uygulamanız gerekir. Bir WebAssembly ana bilgisayarı (IsWasm = true) bunu ayarlamalıdır, çünkü varsayılan dosya önbelleği için yerel disk yoktur.

### RedactionUseClientGenerateId {#RedactionUseClientGenerateId}
```
public boolean RedactionUseClientGenerateId
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
public boolean getAutoFitColumnsOnLoad()
```


Dosya yüklenirken sütun genişliklerinin otomatik ayarlanıp ayarlanmayacağını gösterir, varsayılan değer false'tur.

**Returns:**
boolean
### getAutoFitRowsHeightOnLoad() {#getAutoFitRowsHeightOnLoad--}
```
public boolean getAutoFitRowsHeightOnLoad()
```


Dosya yüklenirken satır yüksekliğinin otomatik ayarlanıp ayarlanmayacağını gösterir, varsayılan değer false'tur.

**Returns:**
boolean
### getAutoOptimizeForLargeCells() {#getAutoOptimizeForLargeCells--}
```
public boolean getAutoOptimizeForLargeCells()
```


Büyük hücreli çalışma sayfası için yük performansını otomatik olarak optimize edip etmeyeceğini alır. Yük süresini azaltmak için bazı stil /kenarları yok sayar. Varsayılan değer true'tir.

**Returns:**
boolean
### getBaseRouteName() {#getBaseRouteName--}
```
public String getBaseRouteName()
```


GridJs denetleyicisi için rota URL temel adını alır. Varsayılan değer GridJs2'dir.

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
public int getEmptySheetMaxCol()
```


Boş bir çalışma sayfası için varsayılan maksimum sütunu alır. Varsayılan değer 15'tir.

**Returns:**
int
### getEmptySheetMaxRow() {#getEmptySheetMaxRow--}
```
public int getEmptySheetMaxRow()
```


Boş bir çalışma sayfası için varsayılan maksimum satırı alır. Varsayılan değer 12'dir.

**Returns:**
int
### getEnableChartClientRendering() {#getEnableChartClientRendering--}
```
public boolean getEnableChartClientRendering()
```


İstemci tarafı grafik render'ını etkinleştirip etkinleştirmeyeceğini alır. False olarak ayarlanırsa, GridJs yalnızca grafik resimleri/şekilleri üretir ve istemci tarafı grafik render'ına ihtiyaç duymaz. Varsayılan değer true'tir.

**Returns:**
boolean
### getFileCacheDirectory() {#getFileCacheDirectory--}
```
public String getFileCacheDirectory()
```


Elektronik tablo dosyasını depolamak için önbellek dizinini alır. GridJs'i kullanmadan önce bunu belirli bir yola ayarlamamız gerekir.

**Returns:**
java.lang.String
### getFontFolders() {#getFontFolders--}
```
public String[] getFontFolders()
```


Render edilen resim/şekillerdeki yazı tipleri için yazı tipi klasörlerini alır.

**Returns:**
java.lang.String[]
### getIgnoreEmptyContent() {#getIgnoreEmptyContent--}
```
public boolean getIgnoreEmptyContent()
```


Veri, stil, birleştirilmiş hücreler ve şekilleri içeren maksimum aralığın gösterilip gösterilmeyeceğini alır. Son satır veya sütun değer ve formül içermeyen ancak özel stil olan hücreler içeriyorsa, bu değer true olduğunda o satır/sütun gösterilmez\u9286?\* Varsayılan değer true'tir.

**Returns:**
boolean
### getIslimitShapeOrImage() {#getIslimitShapeOrImage--}
```
public boolean getIslimitShapeOrImage()
```


Bir çalışma sayfasında toplam görüntülenen şekil/görüntü sayısının sınırlanıp sınırlanmayacağını alır, true olarak ayarlanırsa, GridJs bir çalışma sayfasındaki görüntülenen şekil veya görüntülerin toplam sayısını MaxShapeOrImageCount değerine sınırlar, varsayılan değer true'tır.

**Returns:**
boolean
### getJsonCache() {#getJsonCache--}
```
public JsonCacheOptions getJsonCache()
```


JSON önbellek yapılandırma seçeneklerini alır. Oluşturulan çalışma kitabı JSON'ı için bellek (L1) ve disk (L2) önbellek davranışını kontrol eder.

**Returns:**
[JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions)
### getLazyLoading() {#getLazyLoading--}
```
public boolean getLazyLoading()
```


Yalnızca etkin çalışma sayfasının yüklenip yüklenmeyeceğini alır, varsayılan değer false'tur.

**Returns:**
boolean
### getMaxPdfSaveSeconds() {#getMaxPdfSaveSeconds--}
```
public int getMaxPdfSaveSeconds()
```


PDF'ye kaydederken maksimum zaman aşımı saniyesini alır. Varsayılan değer 10'dur.

**Returns:**
int
### getMaxShapeOrImageCount() {#getMaxShapeOrImageCount--}
```
public int getMaxShapeOrImageCount()
```


Etkin sayfadaki görüntülenen şekil veya resimlerin toplam sayısını alır, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 100'dür.

**Returns:**
int
### getMaxShapeOrImageWidthOrHeight() {#getMaxShapeOrImageWidthOrHeight--}
```
public int getMaxShapeOrImageWidthOrHeight()
```


Bir şekil veya resim için maksimum genişlik veya yüksekliği alır, GridJs bu değerden daha büyük genişlik veya yüksekliğe sahip şekil veya resmi yok sayar, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 10000'dir.

**Returns:**
int
### getMaxTotalShapeOrImageCount() {#getMaxTotalShapeOrImageCount--}
```
public int getMaxTotalShapeOrImageCount()
```


Çalışma kitabındaki görüntülenen şekil veya resimlerin toplam sayısını alır, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 300'dür.

**Returns:**
int
### getMessageTopic() {#getMessageTopic--}
```
public String getMessageTopic()
```


Websocket hedeflerini "\/topic" önekiyle alır. Varsayılan değer "\/topic/opr"'dir. Yalnızca işbirlikçi modda kullanılır.

**Returns:**
java.lang.String
### getPictureCacheDirectory() {#getPictureCacheDirectory--}
```
public String getPictureCacheDirectory()
```


Resimler için önbellek dizinini alır.(bu, GridJsWorkbook.CacheImp null olduğunda etkili olur) Varsayılan yol, FileCacheDirectory içinde "\_piccache" olacaktır.

**Returns:**
java.lang.String
### getSameImageDetecting() {#getSameImageDetecting--}
```
public boolean getSameImageDetecting()
```


Resimlerin aynı kaynağa sahip olup olmadığını kontrol edip etmeyeceğini alır, varsayılan değer true'tır.

**Returns:**
boolean
### getSaveHtmlAsZip() {#getSaveHtmlAsZip--}
```
public boolean getSaveHtmlAsZip()
```


HTML dosyasını zip arşivi olarak kaydedip kaydetmeyeceğini alır, varsayılan değer false'tur.

**Returns:**
boolean
### getShowChartSheet() {#getShowChartSheet--}
```
public boolean getShowChartSheet()
```


Grafik çalışma sayfasının gösterilip gösterilmeyeceğini alır. Varsayılan değer false'tur.

**Returns:**
boolean
### getSkipInvisibleShapes() {#getSkipInvisibleShapes--}
```
public boolean getSkipInvisibleShapes()
```


UI'da görünmez olan şekilleri atlayıp atlamayacağını alır, varsayılan değer true.

**Returns:**
boolean
### getUsePrintArea() {#getUsePrintArea--}
```
public boolean getUsePrintArea()
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
public boolean isCollaborative()
```


Ortak düzenlemeyi destekleyip desteklemeyeceğini alır, varsayılan değer false.

**Returns:**
boolean
### isWasm() {#isWasm--}
```
public boolean isWasm()
```


GridJs'in bir sunucu süreci yerine tarayıcı WebAssembly ana bilgisayarında çalışıp çalışmadığını alır. True olduğunda, FileCacheDirectory / disk / kesinti-iş parçacığı yolu kullanılmaz ve dosya önbelleği CacheImp'ten gelmelidir, çünkü tarayıcı ana bilgisayarının yerel diski yoktur. Çalışma zamanında kod yollarını seçer, böylece tek bir Aspose.Cells.GridJs.dll her iki ana bilgisayarı da hizmet eder. Varsayılan değer false'tur.

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
public void setAutoFitColumnsOnLoad(boolean value)
```


Dosya yüklenirken sütun genişliklerinin otomatik ayarlanıp ayarlanmayacağını gösterir, varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoFitRowsHeightOnLoad(boolean value) {#setAutoFitRowsHeightOnLoad-boolean-}
```
public void setAutoFitRowsHeightOnLoad(boolean value)
```


Dosya yüklenirken satır yüksekliğinin otomatik ayarlanıp ayarlanmayacağını gösterir, varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAutoOptimizeForLargeCells(boolean value) {#setAutoOptimizeForLargeCells-boolean-}
```
public void setAutoOptimizeForLargeCells(boolean value)
```


Büyük hücreli çalışma sayfası için yük performansını otomatik olarak optimize edip etmeyeceğini ayarlar. Yük süresini azaltmak için bazı stil /kenarları yok sayar. Varsayılan değer true'tir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setBaseRouteName(String value) {#setBaseRouteName-java.lang.String-}
```
public void setBaseRouteName(String value)
```


GridJs denetleyicisi için rota URL temel adını ayarlar, varsayılan değer GridJs2.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCollaborative(boolean value) {#setCollaborative-boolean-}
```
public void setCollaborative(boolean value)
```


Ortak düzenlemeyi destekleyip desteklemeyeceğini ayarlar, varsayılan değer false.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEmptySheetMaxCol(int value) {#setEmptySheetMaxCol-int-}
```
public void setEmptySheetMaxCol(int value)
```


Boş bir çalışma sayfası için varsayılan maksimum sütunu ayarlar. Varsayılan değer 15'tir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setEmptySheetMaxRow(int value) {#setEmptySheetMaxRow-int-}
```
public void setEmptySheetMaxRow(int value)
```


Boş bir çalışma sayfası için varsayılan maksimum satırı ayarlar. Varsayılan değer 12'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setEnableChartClientRendering(boolean value) {#setEnableChartClientRendering-boolean-}
```
public void setEnableChartClientRendering(boolean value)
```


İstemci tarafı grafik render'ını etkinleştirip etkinleştirmeyeceğini ayarlar. False olarak ayarlanırsa, GridJs yalnızca grafik resimleri/şekilleri üretir ve istemci tarafı grafik render'ına ihtiyaç duymaz. Varsayılan değer true'tir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFileCacheDirectory(String value) {#setFileCacheDirectory-java.lang.String-}
```
public void setFileCacheDirectory(String value)
```


Elektronik tablo dosyasını depolamak için önbellek dizinini ayarlar. GridJs'i kullanmadan önce bunu belirli bir yola ayarlamamız gerekir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setFontFolders(String[] value) {#setFontFolders-java.lang.String---}
```
public void setFontFolders(String[] value)
```


Render edilmiş resim/şekillerdeki yazı tipleri için yazı tipi klasörlerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String[] |  |

### setIgnoreEmptyContent(boolean value) {#setIgnoreEmptyContent-boolean-}
```
public void setIgnoreEmptyContent(boolean value)
```


Veri, stil, birleştirilmiş hücreler ve şekilleri içeren maksimum aralığın gösterilip gösterilmeyeceğini ayarlar. Son satır veya sütun değer ve formül içermeyen ancak özel stil olan hücreler içeriyorsa, bu değer true olduğunda o satır/sütun gösterilmez\u9286?\* Varsayılan değer true'tir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setIslimitShapeOrImage(boolean value) {#setIslimitShapeOrImage-boolean-}
```
public void setIslimitShapeOrImage(boolean value)
```


Bir çalışma sayfasındaki toplam görüntülenen şekil/görsel sayısını sınırlayıp sınırlamayacağını ayarlar, true olarak ayarlanırsa GridJs, bir çalışma sayfasındaki görüntülenen şekil veya görsel sayısını MaxShapeOrImageCount değerine sınırlar, varsayılan değer true.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setJsonCache(JsonCacheOptions value) {#setJsonCache-com.aspose.gridjs.JsonCacheOptions-}
```
public void setJsonCache(JsonCacheOptions value)
```


JSON önbellek yapılandırma seçeneklerini ayarlar. Oluşturulan çalışma kitabı JSON'ı için hem bellek (L1) hem de disk (L2) önbellek davranışını kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions) |  |

### setLazyLoading(boolean value) {#setLazyLoading-boolean-}
```
public void setLazyLoading(boolean value)
```


Yalnızca aktif çalışma sayfasını yükleyip yüklemeyeceğini ayarlar, varsayılan değer false.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMaxPdfSaveSeconds(int value) {#setMaxPdfSaveSeconds-int-}
```
public void setMaxPdfSaveSeconds(int value)
```


PDF'ye kaydedilirken maksimum zaman aşımı saniyesini ayarlar. Varsayılan değer 10'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMaxShapeOrImageCount(int value) {#setMaxShapeOrImageCount-int-}
```
public void setMaxShapeOrImageCount(int value)
```


Etkin sayfadaki görüntülenen şekil veya resimlerin toplam sayısını ayarlar, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 100'dür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMaxShapeOrImageWidthOrHeight(int value) {#setMaxShapeOrImageWidthOrHeight-int-}
```
public void setMaxShapeOrImageWidthOrHeight(int value)
```


Bir şekil veya resim için maksimum genişlik veya yüksekliği ayarlar, GridJs bu genişlik veya yüksekliği aşan şekil veya resmi yok sayar, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 10000'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMaxTotalShapeOrImageCount(int value) {#setMaxTotalShapeOrImageCount-int-}
```
public void setMaxTotalShapeOrImageCount(int value)
```


Çalışma kitabındaki görüntülenen şekil veya resimlerin toplam sayısını ayarlar, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 300'dür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setMessageTopic(String value) {#setMessageTopic-java.lang.String-}
```
public void setMessageTopic(String value)
```


Websocket hedeflerini "/topic" önekiyle ayarlar. Varsayılan değer "/topic/opr". Yalnızca ortak çalışma modunda kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPictureCacheDirectory(String value) {#setPictureCacheDirectory-java.lang.String-}
```
public void setPictureCacheDirectory(String value)
```


Resimler için önbellek dizinini ayarlar. (Bu, GridJsWorkbook.CacheImp null olduğunda etkili olur) Varsayılan yol, FileCacheDirectory içinde "\_piccache" olacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setSameImageDetecting(boolean value) {#setSameImageDetecting-boolean-}
```
public void setSameImageDetecting(boolean value)
```


Resimlerin aynı kaynağa sahip olup olmadığını kontrol edip etmeyeceğini ayarlar, varsayılan değer true.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSaveHtmlAsZip(boolean value) {#setSaveHtmlAsZip-boolean-}
```
public void setSaveHtmlAsZip(boolean value)
```


HTML dosyasını zip arşivi olarak kaydedip kaydetmeyeceğini ayarlar, varsayılan değer false.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setShowChartSheet(boolean value) {#setShowChartSheet-boolean-}
```
public void setShowChartSheet(boolean value)
```


Grafik çalışma sayfasının gösterilip gösterilmeyeceğini ayarlar. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSkipInvisibleShapes(boolean value) {#setSkipInvisibleShapes-boolean-}
```
public void setSkipInvisibleShapes(boolean value)
```


UI için görünmez olan şekilleri atlayıp atlamayacağını ayarlar, varsayılan değer true'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setUsePrintArea(boolean value) {#setUsePrintArea-boolean-}
```
public void setUsePrintArea(boolean value)
```


Çalışma sayfasının PrintArea için PageSetup ayarı olduğunda UI görüntüleme aralığı için PageSetup.PrintArea kullanılmasını ayarlar. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setWasm(boolean value) {#setWasm-boolean-}
```
public void setWasm(boolean value)
```


GridJs'nin bir sunucu süreci yerine bir tarayıcı WebAssembly ana bilgisayarında çalışıp çalışmayacağını ayarlar. True olduğunda, FileCacheDirectory / disk / interrupt-thread yolu kullanılmaz ve dosya önbelleği CacheImp'ten gelmelidir, çünkü tarayıcı ana bilgisayarının yerel diski yoktur. Çalışma zamanında kod yollarını seçer, böylece tek bir Aspose.Cells.GridJs.dll her iki ana bilgisayarı da hizmet eder. Varsayılan değer false'tur.

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


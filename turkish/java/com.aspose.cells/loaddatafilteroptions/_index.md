---
title: "LoadDataFilterOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Şablondan çalışma kitabı yüklenirken verileri filtreleme seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/loaddatafilteroptions/
---

**Inheritance:**
java.lang.Object
```
public final class LoadDataFilterOptions
```

Şablondan çalışma kitabı yüklenirken verileri filtreleme seçeneklerini temsil eder.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [ALL](#ALL) | Hepsini yükle |
| [BOOK_SETTINGS](#BOOK-SETTINGS) | Çalışma kitabı ayarlarını yükle |
| [CELL_BLANK](#CELL-BLANK) | Değeri boş olan hücreleri yükle |
| [CELL_BOOL](#CELL-BOOL) | Değeri bool olan hücreleri yükle |
| [CELL_DATA](#CELL-DATA) | Değerleri, formülleri ve biçimlendirmeyi içeren hücre verilerini yükle |
| [CELL_ERROR](#CELL-ERROR) | Değeri hata olan hücreleri yükle |
| [CELL_NUMERIC](#CELL-NUMERIC) | Değeri sayısal (tarih ve saat dahil) olan hücreleri yükle |
| [CELL_STRING](#CELL-STRING) | Değeri metin olan hücreleri yükle |
| [CELL_VALUE](#CELL-VALUE) | Yalnızca hücre değerlerini (tüm değer tipleri) yükle |
| [CHART](#CHART) | Grafikleri yükle |
| [CONDITIONAL_FORMATTING](#CONDITIONAL-FORMATTING) | Koşullu biçimlendirmeyi yükle |
| [DATA_VALIDATION](#DATA-VALIDATION) | Veri doğrulamalarını yükle |
| [DEFINED_NAMES](#DEFINED-NAMES) | Tanımlı Ad nesnelerini yükle |
| [DOCUMENT_PROPERTIES](#DOCUMENT-PROPERTIES) | Belge özelliklerini yükle |
| [DRAWING](#DRAWING) | Çizim nesneleri (Grafik, Resim, OleObject ve diğer tüm çizim nesneleri dahil) |
| [FORMULA](#FORMULA) | Hücre formüllerini yükle. |
| [HYPERLINKS](#HYPERLINKS) | Köprüleri yükle |
| [MERGED_AREA](#MERGED-AREA) | Birleştirilmiş hücreleri yükle |
| [NONE](#NONE) | Sayfa verileri için hiçbir şey yükleme |
| [OLE_OBJECT](#OLE-OBJECT) | OleObjects'ı yükle |
| [PICTURE](#PICTURE) | Resimleri yükle |
| [PIVOT_TABLE](#PIVOT-TABLE) | Pivot tablolarını yükle |
| [REVISION](#REVISION) | Revizyon günlüklerini yükle |
| [SETTINGS](#SETTINGS) | Çalışma kitabı ve çalışma sayfası ayarlarını yükle |
| [SHAPE](#SHAPE) | Şekilleri yükle |
| [SHEET_DATA](#SHEET-DATA) | Çalışma sayfasının tüm verilerini, örneğin hücre verileri, ayarlar, nesneler, ... vb. yükle |
| [SHEET_SETTINGS](#SHEET-SETTINGS) | Çalışma sayfası ayarlarını yükle |
| [STRUCTURE](#STRUCTURE) | Çalışma kitabının yapısını yükle |
| [STYLE](#STYLE) | Hücre biçimlendirme stillerini yükle |
| [TABLE](#TABLE) | Tabloları yükle |
| [VBA](#VBA) | VBA projelerini yükle |
| [XML_MAP](#XML-MAP) | XmlMap'i Yükle |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL {#ALL}
```
public static final int ALL
```


Hepsini yükle

### BOOK_SETTINGS {#BOOK-SETTINGS}
```
public static final int BOOK_SETTINGS
```


Çalışma kitabı ayarlarını yükle

### CELL_BLANK {#CELL-BLANK}
```
public static final int CELL_BLANK
```


Değeri boş olan hücreleri yükle

### CELL_BOOL {#CELL-BOOL}
```
public static final int CELL_BOOL
```


Değeri bool olan hücreleri yükle

### CELL_DATA {#CELL-DATA}
```
public static final int CELL_DATA
```


Değerleri, formülleri ve biçimlendirmeyi içeren hücre verilerini yükle

### CELL_ERROR {#CELL-ERROR}
```
public static final int CELL_ERROR
```


Değeri hata olan hücreleri yükle

### CELL_NUMERIC {#CELL-NUMERIC}
```
public static final int CELL_NUMERIC
```


Değeri sayısal (tarih ve saat dahil) olan hücreleri yükle

### CELL_STRING {#CELL-STRING}
```
public static final int CELL_STRING
```


Değeri metin olan hücreleri yükle

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


Yalnızca hücre değerlerini (tüm değer tipleri) yükle

### CHART {#CHART}
```
public static final int CHART
```


Grafikleri yükle

### CONDITIONAL_FORMATTING {#CONDITIONAL-FORMATTING}
```
public static final int CONDITIONAL_FORMATTING
```


Koşullu biçimlendirmeyi yükle

### DATA_VALIDATION {#DATA-VALIDATION}
```
public static final int DATA_VALIDATION
```


Veri doğrulamalarını yükle

### DEFINED_NAMES {#DEFINED-NAMES}
```
public static final int DEFINED_NAMES
```


Tanımlı Ad nesnelerini yükle

### DOCUMENT_PROPERTIES {#DOCUMENT-PROPERTIES}
```
public static final int DOCUMENT_PROPERTIES
```


Belge özelliklerini yükle

### DRAWING {#DRAWING}
```
public static final int DRAWING
```


Çizim nesneleri (Grafik, Resim, OleObject ve diğer tüm çizim nesneleri dahil)

### FORMULA {#FORMULA}
```
public static final int FORMULA
```


Hücre formüllerini yükle.

**Remarks**

Genel olarak tanımlı Ad nesneleri (DefinedNames) formüller yüklenirken de yüklenmelidir çünkü formüller tarafından referans alınabilirler. Bu nedenle Formula veya CellData seçeneği, çoğu senaryo için DefinedNames seçeneğiyle birlikte (Formula\|DefinedNames veya CellData\|DefinedNames) çalışmalıdır.

### HYPERLINKS {#HYPERLINKS}
```
public static final int HYPERLINKS
```


Köprüleri yükle

### MERGED_AREA {#MERGED-AREA}
```
public static final int MERGED_AREA
```


Birleştirilmiş hücreleri yükle

### NONE {#NONE}
```
public static final int NONE
```


Sayfa verileri için hiçbir şey yükleme

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır ve lütfen yerine Structure kullanın. Bu özellik Aralık 2017'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### OLE_OBJECT {#OLE-OBJECT}
```
public static final int OLE_OBJECT
```


OleObjects'ı yükle

### PICTURE {#PICTURE}
```
public static final int PICTURE
```


Resimleri yükle

### PIVOT_TABLE {#PIVOT-TABLE}
```
public static final int PIVOT_TABLE
```


Pivot tablolarını yükle

### REVISION {#REVISION}
```
public static final int REVISION
```


Revizyon günlüklerini yükle

### SETTINGS {#SETTINGS}
```
public static final int SETTINGS
```


Çalışma kitabı ve çalışma sayfası ayarlarını yükle

### SHAPE {#SHAPE}
```
public static final int SHAPE
```


Şekilleri yükle

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır ve lütfen yerine Drawing kullanın. Bu özellik Kasım 2019'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### SHEET_DATA {#SHEET-DATA}
```
public static final int SHEET_DATA
```


Çalışma sayfasının tüm verilerini, örneğin hücre verileri, ayarlar, nesneler, ... vb. yükle

### SHEET_SETTINGS {#SHEET-SETTINGS}
```
public static final int SHEET_SETTINGS
```


Çalışma sayfası ayarlarını yükle

### STRUCTURE {#STRUCTURE}
```
public static final int STRUCTURE
```


Çalışma kitabının yapısını yükle

### STYLE {#STYLE}
```
public static final int STYLE
```


Hücre biçimlendirme stillerini yükle

### TABLE {#TABLE}
```
public static final int TABLE
```


Tabloları yükle

### VBA {#VBA}
```
public static final int VBA
```


VBA projelerini yükle

### XML_MAP {#XML-MAP}
```
public static final int XML_MAP
```


XmlMap'i Yükle

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
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




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


---
title: "GridTxtLoadOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Metin dosyası yükleme seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/gridtxtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
```
public class GridTxtLoadOptions extends GridLoadOptions
```

Metin dosyası yükleme seçeneklerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GridTxtLoadOptions()](#GridTxtLoadOptions--) | Metin dosyasını yüklemek için seçenekleri oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmediğini gösterir. |
| [getCheckDataValid()](#getCheckDataValid--) | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Metin dosyasındaki dizgenin tarih verisine dönüştürülüp dönüştürülmediğini gösteren bir değer alır. |
| [getConvertNumericData()](#getConvertNumericData--) | Metin dosyasındaki dizgenin sayısal veriye dönüştürülüp dönüştürülmediğini gösteren bir değer alır. |
| [getEncoding()](#getEncoding--) | Varsayılan kodlamayı alır. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | Veri satırları veya sütunları limit aşınca veriyi bir sonraki sayfaya genişletip genişletmeyeceğini belirler. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Dosyayı doğrudan yazdırırken yazdırılmayan verileri yoksayar |
| [getKeepPrecision()](#getKeepPrecision--) | Uzunluğu 15 ise dize değerinin ayrılmayacağını gösterir. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Şablon dosyasından yüklendiğinde Çalışma Kitabı için ayrıştırılmamış verilerin bellekte tutulup tutulmadığını gösterir. |
| [getOnlyAuto()](#getOnlyAuto--) | Satır yüksekliği özelleştirilmemiş olan satırların yalnızca sığdırılıp sığdırılmayacağını gösterir. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Dosya okunurken formülün ayrıştırılıp ayrıştırılmadığını gösterir. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmadığını gösterir. |
| [getPassword()](#getPassword--) | Çalışma kitabının şifresini alır. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşluk ve satır sonlarının korunup korunmadığını gösterir. |
| [getSeparator()](#getSeparator--) | Metin dosyasının karakter ayırıcıyı alır. |
| [getSeparatorString()](#getSeparatorString--) | Ayırıcı olarak bir dize değeri alır. |
| [getTextQualifier()](#getTextQualifier--) | Hücre değerleri için metin niteleyicisini belirtir. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | Ardışık sınırlayıcıların tek olarak değerlendirilip değerlendirilmeyeceği. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | Başlangıçtaki tek tırnak işaretinin bir hücrenin değeriyle birlikte alınması gerekip gerekmediğini gösterir. |
| [hasFormula()](#hasFormula--) | Metnin "=" ile başlaması durumunda formül olup olmadığını gösterir. |
| [hasTextQualifier()](#hasTextQualifier--) | Hücre değeri için metin niteleyicisinin olup olmadığı. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | Doğru, dosyanın birden fazla kodlama içerdiği anlamına gelir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmediğini gösterir. |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediğini gösterir. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Metin dosyasındaki dizeyin tarih verisine dönüştürülüp dönüştürülmeyeceğini gösteren bir değer ayarlar. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Metin dosyasındaki dizeyin sayısal veriye dönüştürülüp dönüştürülmeyeceğini gösteren bir değer ayarlar. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | Varsayılan kodlamayı ayarlar. |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | Veri satırları veya sütunları limit aşınca veriyi bir sonraki sayfaya genişletip genişletmeyeceğini belirler. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Metnin "=" ile başlaması durumunda formül olup olmadığını gösterir. |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | Hücre değeri için metin niteleyicisinin olup olmadığı. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Dosyayı doğrudan yazdırırken yazdırılmayan verileri yoksayar |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Uzunluğu 15 ise dize değerinin ayrılmayacağını gösterir. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Şablon dosyasından yüklendiğinde Çalışma Kitabı için ayrıştırılmamış verilerin bellekte tutulup tutulmadığını gösterir. |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | Doğru, dosyanın birden fazla kodlama içerdiği anlamına gelir. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Satır yüksekliği özelleştirilmemiş olan satırların yalnızca sığdırılıp sığdırılmayacağını gösterir. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Dosya okunurken formülün ayrıştırılıp ayrıştırılmadığını gösterir. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmadığını gösterir. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Workbook'un şifresini ayarlar. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşluk ve satır sonlarının korunup korunmadığını gösterir. |
| [setSeparator(char value)](#setSeparator-char-) | Metin dosyasının karakter ayırıcıyı ayarlar. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Ayırıcı olarak bir dize değeri ayarlar. |
| [setTextQualifier(char value)](#setTextQualifier-char-) | Hücre değerleri için metin niteleyicisini belirtir. |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | Ardışık sınırlayıcıların tek olarak değerlendirilip değerlendirilmeyeceği. |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | Başlangıçtaki tek tırnak işaretinin bir hücrenin değeriyle birlikte alınması gerekip gerekmediğini gösterir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTxtLoadOptions() {#GridTxtLoadOptions--}
```
public GridTxtLoadOptions()
```


Metin dosyasını yüklemek için seçenekleri oluşturur.

**Remarks**

Varsayılan yükleme dosya türü CSV'dir.

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
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmediğini gösterir.

**Remarks**

Bazen otomatik filtre ayarlı olsa da ilgili satırlar dosyada gizlenmez. Şimdi yalnızca SpreadSheetML dosyası için çalışır.

**Returns:**
boolean
### getCheckDataValid() {#getCheckDataValid--}
```
public boolean getCheckDataValid()
```


Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi bir yöntemle 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir İstisna alırsınız. Bu özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, Excel dosya formatı için geçersiz bir değer ayarladıysanız, workbook'u daha sonra Excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan Excel dosyasında beklenmeyen hatalar oluşabilir.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertDateTimeData() {#getConvertDateTimeData--}
```
public boolean getConvertDateTimeData()
```


Metin dosyasındaki dizgenin tarih verisine dönüştürülüp dönüştürülmediğini gösteren bir değer alır.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Metin dosyasındaki dizgenin sayısal veriye dönüştürülüp dönüştürülmediğini gösteren bir değer alır.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Varsayılan kodlamayı alır. Yalnızca csv dosyası için geçerlidir.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


Veri satırları veya sütunları limit aşınca verinin bir sonraki sayfaya genişletilip genişletilmeyeceğini belirler. Bu özellik true ise, ekstra veri mevcut sayfanın arkasındaki bir sonraki sayfaya genişletilir (eğer mevcut sayfa son sayfa ise, yeni bir sayfa mevcut çalışma kitabına eklenir). Bu özellik false ise, limit aşan veri yok sayılır. Varsayılan değer false;

**Returns:**
boolean
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Dosyayı doğrudan yazdırırken yazdırılmayan verileri yoksayar

**Remarks**

Yalnızca xlsx dosyası için.

**Returns:**
boolean
### getKeepPrecision() {#getKeepPrecision--}
```
public boolean getKeepPrecision()
```


Uzunluğu 15 ise dize değerinin ayrılmayacağını gösterir.

**Returns:**
boolean
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```


Workbook bir şablon dosyasından yüklendiğinde ayrıştırılmamış verilerin bellekte tutulup tutulmayacağı. Varsayılan değer true'tur.

**Remarks**

Kullanıcının yalnızca şablon dosyasından bazı içerikleri okuması ve workbook'u geri kaydetmeye ihtiyacı olmadığı senaryolarda, bu özelliği false olarak ayarlamak performansı artırabilir, özellikle bir tür LoadFilter ile birlikte kullanıldığında.

**Returns:**
boolean
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Satır yüksekliği özelleştirilmemiş olan satırların yalnızca sığdırılıp sığdırılmayacağını gösterir.

**Returns:**
boolean
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


Dosya okunurken formülün ayrıştırılıp ayrıştırılmadığını gösterir.

**Remarks**

Yalnızca Excel Xlsx, Xltx, Xltm ve Xlsm dosyalarına uygulanır çünkü dosyalardaki formüller dize formülü olarak depolanır.

**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```


Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmayacağını gösterir. Varsayılan değer false'tur.

**Remarks**

Yalnızca Excel Xlsx, Xltx, Xltm, Xlsm ve xlsb dosyalarına uygulanır.

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


Çalışma kitabının şifresini alır.

**Returns:**
java.lang.String
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Formülleri alırken ve ayarlarken formül tokenları arasında doldurulan boşlukları ve satır sonlarını koruyup korumayacağını gösterir. Varsayılan değer false'tur.

**Remarks**

Bu seçenekle şablon dosyasından çalışma kitabı yüklendikten sonra, [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\#getPreservePaddingSpaces--) aynı değerle bu özelliğe ayarlanacaktır.

**Returns:**
boolean
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Metin dosyasının karakter ayırıcıyı alır.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Ayırıcı olarak bir dize değeri alır.

**Returns:**
java.lang.String
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


Hücre değerleri için metin niteleyicisini belirtir. Varsayılan niteleyici '"'dir.

**Remarks**

Bu özellik ayarlandığında, [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) otomatik olarak true olur.

**Returns:**
char
### getTreatConsecutiveDelimitersAsOne() {#getTreatConsecutiveDelimitersAsOne--}
```
public boolean getTreatConsecutiveDelimitersAsOne()
```


Ardışık sınırlayıcıların tek olarak değerlendirilip değerlendirilmeyeceği.

**Returns:**
boolean
### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}
```
public boolean getTreatQuotePrefixAsValue()
```


Bir hücrenin değerinin bir parçası olarak baştaki tek tırnak işaretinin alınması gerekip gerekmediğini gösterir. Varsayılan değer true'tır. False ise, baştaki tek tırnak ilgili hücrenin değerinden kaldırılır ve [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) hücre için true olarak ayarlanır.

**Returns:**
boolean
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```


Metnin "=" ile başlaması durumunda formül olup olmadığını gösterir.

**Returns:**
boolean
### hasTextQualifier() {#hasTextQualifier--}
```
public boolean hasTextQualifier()
```


Hücre değeri için metin niteleyicisinin olup olmadığı. Varsayılan değer true.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMultiEncoded() {#isMultiEncoded--}
```
public boolean isMultiEncoded()
```


Doğru, dosyanın birden fazla kodlama içerdiği anlamına gelir.

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




### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```


Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmediğini gösterir.

**Remarks**

Bazen otomatik filtre ayarlı olsa da ilgili satırlar dosyada gizlenmez. Şimdi yalnızca SpreadSheetML dosyası için çalışır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi bir yöntemle 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir İstisna alırsınız. Bu özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, Excel dosya formatı için geçersiz bir değer ayarladıysanız, workbook'u daha sonra Excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan Excel dosyasında beklenmeyen hatalar oluşabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```


Metin dosyasındaki dizeyin tarih verisine dönüştürülüp dönüştürülmeyeceğini gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Metin dosyasındaki dizeyin sayısal veriye dönüştürülüp dönüştürülmeyeceğini gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


Varsayılan kodlamayı ayarlar. Yalnızca csv dosyaları için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


Veri satırları veya sütunları limit aşınca verinin bir sonraki sayfaya genişletilip genişletilmeyeceğini belirler. Bu özellik true ise, ekstra veri mevcut sayfanın arkasındaki bir sonraki sayfaya genişletilir (eğer mevcut sayfa son sayfa ise, yeni bir sayfa mevcut çalışma kitabına eklenir). Bu özellik false ise, limit aşan veri yok sayılır. Varsayılan değer false;

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```


Metnin "=" ile başlaması durumunda formül olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasTextQualifier(boolean value) {#setHasTextQualifier-boolean-}
```
public void setHasTextQualifier(boolean value)
```


Hücre değeri için metin niteleyicisinin olup olmadığı. Varsayılan değer true.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


Dosyayı doğrudan yazdırırken yazdırılmayan verileri yoksayar

**Remarks**

Yalnızca xlsx dosyası için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```


Uzunluğu 15 ise dize değerinin ayrılmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


Workbook bir şablon dosyasından yüklendiğinde ayrıştırılmamış verilerin bellekte tutulup tutulmayacağı. Varsayılan değer true'tur.

**Remarks**

Kullanıcının yalnızca şablon dosyasından bazı içerikleri okuması ve workbook'u geri kaydetmeye ihtiyacı olmadığı senaryolarda, bu özelliği false olarak ayarlamak performansı artırabilir, özellikle bir tür LoadFilter ile birlikte kullanıldığında.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


Doğru, dosyanın birden fazla kodlama içerdiği anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Satır yüksekliği özelleştirilmemiş olan satırların yalnızca sığdırılıp sığdırılmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


Dosya okunurken formülün ayrıştırılıp ayrıştırılmadığını gösterir.

**Remarks**

Yalnızca Excel Xlsx, Xltx, Xltm ve Xlsm dosyalarına uygulanır çünkü dosyalardaki formüller dize formülü olarak depolanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmayacağını gösterir. Varsayılan değer false'tur.

**Remarks**

Yalnızca Excel Xlsx, Xltx, Xltm, Xlsm ve xlsb dosyalarına uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Workbook'un şifresini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


Formülleri alırken ve ayarlarken formül tokenları arasında doldurulan boşlukları ve satır sonlarını koruyup korumayacağını gösterir. Varsayılan değer false'tur.

**Remarks**

Bu seçenekle şablon dosyasından çalışma kitabı yüklendikten sonra, [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\#getPreservePaddingSpaces--) aynı değerle bu özelliğe ayarlanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Metin dosyasının karakter ayırıcıyı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


Ayırıcı olarak bir dize değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


Hücre değerleri için metin niteleyicisini belirtir. Varsayılan niteleyici '"'dir.

**Remarks**

Bu özellik ayarlandığında, [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) otomatik olarak true olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char |  |

### setTreatConsecutiveDelimitersAsOne(boolean value) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```
public void setTreatConsecutiveDelimitersAsOne(boolean value)
```


Ardışık sınırlayıcıların tek olarak değerlendirilip değerlendirilmeyeceği.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setTreatQuotePrefixAsValue(boolean value) {#setTreatQuotePrefixAsValue-boolean-}
```
public void setTreatQuotePrefixAsValue(boolean value)
```


Bir hücrenin değerinin bir parçası olarak baştaki tek tırnak işaretinin alınması gerekip gerekmediğini gösterir. Varsayılan değer true'tır. False ise, baştaki tek tırnak ilgili hücrenin değerinden kaldırılır ve [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) hücre için true olarak ayarlanır.

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


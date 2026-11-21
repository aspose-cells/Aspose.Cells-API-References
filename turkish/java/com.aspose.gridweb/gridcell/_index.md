---
title: "GridCell"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir hücre nesnesini temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/gridcell/
---

**Inheritance:**
java.lang.Object
```
public class GridCell
```

Bir hücre nesnesini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [containsExternalLink()](#containsExternalLink--) | Bu hücrenin harici bir bağlantı içerip içermediğini gösterir. |
| [copy(GridCell source)](#copy-com.aspose.gridweb.GridCell-) | Kaynak hücreden verileri kopyalar. |
| [copyStyle(GridTableItemStyle style)](#copyStyle-com.aspose.gridweb.GridTableItemStyle-) | Stili kopyala ve hücre için stili ayarla |
| [createComment(String note, String author, boolean isvisible)](#createComment-java.lang.String-java.lang.String-boolean-) | Bir hücre için yorum nesnesi oluşturur. |
| [createValidation(int validationType, boolean isRequried)](#createValidation-int-boolean-) | Bir hücre için doğrulama nesnesi oluşturur. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu nesnenin başka bir hücre nesnesiyle aynı hücreye referans verip vermediğini kontrol eder. |
| [getBoolValue()](#getBoolValue--) | Hücrede bulunan boolean değeri alır. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Hücrenin sütun numarasını (sıfır tabanlı) alır. |
| [getComment()](#getComment--) | Bu hücredeki yorum nesnesini al |
| [getDateValue()](#getDateValue--) | Hücrede bulunan DateTime değerini alır. |
| [getDisplayStringValue()](#getDisplayStringValue--) | Bu hücrenin biçimlendirilmiş dize değerini alır. |
| [getDoubleValue()](#getDoubleValue--) | Hücrede bulunan double değerini al. |
| [getFloatValue()](#getFloatValue--) | Hücrede bulunan float değerini al. |
| [getFormula()](#getFormula--) | Bir [GridCell](../../com.aspose.gridweb/gridcell) formülü alır. |
| [getHtmlString()](#getHtmlString--) | Bu hücredeki veri ve bazı biçimlendirmeleri içeren html dizesini alır. |
| [getIntValue()](#getIntValue--) | Hücrede bulunan tam sayı değerini al. |
| [getName()](#getName--) | Hücrenin adını alır. |
| [getRow()](#getRow--) | Hücrenin satır numarasını (sıfır tabanlı) al. |
| [getStringValue()](#getStringValue--) | Hücrede bulunan dize değerini al. |
| [getStyle()](#getStyle--) | Hücre stilinin kopyasını alır. Hücre için stili ayarla. |
| [getType()](#getType--) | Hücre değer tipini döndürür, anlamı GridCellValueType.java dosyasında görülebilir. |
| [getValue()](#getValue--) | Bu hücrede bulunan değeri al. |
| [getWidthOfValue()](#getWidthOfValue--) | Değerin genişliğini piksel biriminde alır. |
| [hashCode()](#hashCode--) | Belirli bir tür için bir karma işlevi olarak hizmet verir. |
| [isErrorValue()](#isErrorValue--) | Bir formülün sonucu düzgün bir şekilde değerlendirebilir olup olmadığını kontrol eder. |
| [isFormula()](#isFormula--) | Belirtilen hücrenin formül içerip içermediğini temsil eder. |
| [isStyleSet()](#isStyleSet--) | Hücrenin stilinin ayarlanıp ayarlanmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean param_boolean)](#putValue-boolean-) | Hücreye bir boolean değer koyar. |
| [putValue(DateTime param_date)](#putValue-com.aspose.gridweb.DateTime-) | Hücreye bir DateTime değeri koyar. |
| [putValue(double param_double)](#putValue-double-) | Hücreye bir double değeri koyar. |
| [putValue(int param_int)](#putValue-int-) | Hücreye bir int değeri koyar. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | Hücreye bir nesne değeri koyar. setValue(Object param\_object) ile aynı. |
| [putValue(String param_string)](#putValue-java.lang.String-) | Hücreye bir String değeri koyar. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | Hücreye bir dize değeri koyar ve uygun olduğunda değeri başka bir veri tipine dönüştürür. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Hücreye bir değer koyar, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır. |
| [putValueAndSetFormatByValue(String stringValue)](#putValueAndSetFormatByValue-java.lang.String-) | Hücrenin değerini bir dize değeriyle ayarlar ve hücre formatını bu değerle belirler. |
| [removeComment()](#removeComment--) | Hücrenin yorum nesnesini kaldırır. |
| [removeValidation()](#removeValidation--) | Hücrenin doğrulama nesnesini kaldırır. |
| [setBorder(WebBorderStyle borderStyle)](#setBorder-com.aspose.gridweb.WebBorderStyle-) | Bir hücre için kenarlıkları (üst, alt, sol ve sağ) ayarlar, tüm kenarlıkların aynı kenarlık stiline sahip olması. |
| [setCustom(String custom)](#setCustom-java.lang.String-) | Özel biçimi ayarlar, null veya boş dize özel biçim olmadığı anlamına gelir. |
| [setFormula(String value)](#setFormula-java.lang.String-) | [GridCell](../../com.aspose.gridweb/gridcell) için bir formül ayarlar. |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | Formülü ve formülün değerini ayarla. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Bu hücredeki veri ve bazı biçimlendirmeleri içeren html dizesini ayarlar. |
| [setNumberType(int numbertype)](#setNumberType-int-) | Sayıların ve tarihlerin görüntüleme biçimini ayarla |
| [setStyle(GridTableItemStyle value)](#setStyle-com.aspose.gridweb.GridTableItemStyle-) | Hücre stilinin kopyasını alır. Hücre için stili ayarla. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Bu hücrede bulunan değeri al. |
| [toString()](#toString--) | Geçerli Cell nesnesini temsil eden bir dize döndürür. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


Bu hücrenin harici bir bağlantı içerip içermediğini gösterir. Yalnızca hücre bir formül hücresi olduğunda uygulanır.

**Returns:**
boolean
### copy(GridCell source) {#copy-com.aspose.gridweb.GridCell-}
```
public void copy(GridCell source)
```


Kaynak hücreden verileri kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [GridCell](../../com.aspose.gridweb/gridcell) | Kaynak [GridCell](../../com.aspose.gridweb/gridcell) nesnesi. |

### copyStyle(GridTableItemStyle style) {#copyStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void copyStyle(GridTableItemStyle style)
```


Stili kopyala ve hücre için stili ayarla

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Kaynak stil. |

### createComment(String note, String author, boolean isvisible) {#createComment-java.lang.String-java.lang.String-boolean-}
```
public GridComment createComment(String note, String author, boolean isvisible)
```


Bir hücre için yorum nesnesi oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| not | java.lang.String | yorum notu. |
| yazar | java.lang.String | yorum yazarı. |
| isvisible | boolean | yorumun görünür olup olmadığını. |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - GridComment object
### createValidation(int validationType, boolean isRequried) {#createValidation-int-boolean-}
```
public GridValidation createValidation(int validationType, boolean isRequried)
```


Bir hücre için doğrulama nesnesi oluşturur.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheet sheet = GridWeb1.getActiveSheet();
         GridValidation v = sheet.getCells().get("A1").createValidation(GridValidationType.CUSTOM_EXPRESSION, true);
         		// Sets to number validation expression.
         		v.setRegEx("\\d+");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| validationType | int | [GridValidationType](../../com.aspose.gridweb/gridvalidationtype). Doğrulama türü. |
| isRequried | boolean | Hücre değerinin gerekli olup olmadığını. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - 
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bu nesnenin başka bir hücre nesnesiyle aynı hücreye referans verip vermediğini kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | başka bir GridCell nesnesi |

**Returns:**
boolean - iki hücre nesnesi aynı hücreye işaret ediyorsa true.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


Hücrede bulunan boolean değeri alır.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Hücrenin sütun numarasını (sıfır tabanlı) alır.

**Returns:**
int
### getComment() {#getComment--}
```
public GridComment getComment()
```


Bu hücredeki yorum nesnesini al

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment)
### getDateValue() {#getDateValue--}
```
public DateTime getDateValue()
```


Hücrede bulunan DateTime değerini alır.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime)
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


Bu hücrenin biçimlendirilmiş dize değerini alır.

**Returns:**
java.lang.String
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Hücrede bulunan double değerini al.

**Returns:**
double
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


Hücrede bulunan float değerini al.

**Returns:**
float
### getFormula() {#getFormula--}
```
public String getFormula()
```


Bir [GridCell](../../com.aspose.gridweb/gridcell) formülü alır.

**Remarks**

Bir formül dizesi her zaman eşittir işareti (=) ile başlar. Ve lütfen parametre ayırıcı olarak her zaman virgül(,) kullanın, örneğin "=SUM(A1, E1, H2)".

Kullanıcı, Workbook tasarım dosyasında herhangi bir formül ayarlayabilir. Aspose.Cells tüm formülleri korur. Kullanıcı bu özelliği bir hücreye formül ayarlamak için kullanırsa, Workbook yerleşik fonksiyonlarının büyük bir kısmı desteklenir. Ve daha fazlası geliyor. Workbook yerleşik fonksiyonları için özel bir ihtiyacınız varsa, lütfen bize bildirin.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheet sheet = GridWeb1.getActiveSheet();
         sheet.getCells().get("B6").setFormula("=SUM(B2:B5, E1) + sheet1!A1");
```

**Returns:**
java.lang.String
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


Bu hücredeki veri ve bazı biçimlendirmeleri içeren html dizesini alır.

**Returns:**
java.lang.String
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


Hücrede bulunan tam sayı değerini al.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Hücrenin adını alır. Örneğin: A1, F102.

**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```


Hücrenin satır numarasını (sıfır tabanlı) al.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Hücrede bulunan dize değerini al.

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public GridTableItemStyle getStyle()
```


Hücre stilinin kopyasını alır. Hücre için stili ayarla.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) - Style object.
### getType() {#getType--}
```
public int getType()
```


Hücre değer tipini döndürür, anlamı GridCellValueType.java dosyasında görülebilir.

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Bu hücrede bulunan değeri al.

**Remarks**

Olası tip:

null,

Boolean,

DateTime,

Double,

Integer

String.

**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```


Değerin genişliğini piksel biriminde alır.

**Returns:**
int -
### hashCode() {#hashCode--}
```
public int hashCode()
```


Belirli bir tür için bir karma işlevi olarak hizmet verir.

**Returns:**
int - Mevcut GridCell nesnesi için bir karma kodu.
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


Bir formülün sonucu düzgün bir şekilde değerlendirebilir olup olmadığını kontrol eder.

**Remarks**

Yalnızca formül hücresi için geçerlidir.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Belirtilen hücrenin formül içerip içermediğini temsil eder.

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


Hücrenin stilinin ayarlanıp ayarlanmadığını gösterir. False dönerse, bu hücrenin varsayılan hücre biçimine sahip olduğu anlamına gelir.

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




### putValue(boolean param_boolean) {#putValue-boolean-}
```
public void putValue(boolean param_boolean)
```


Hücreye bir boolean değer koyar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| param_boolean | boolean | Girdi değeri |

### putValue(DateTime param_date) {#putValue-com.aspose.gridweb.DateTime-}
```
public void putValue(DateTime param_date)
```


Hücreye bir DateTime değeri koyar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| param_date | [DateTime](../../com.aspose.gridweb/datetime) | Girdi değeri |

### putValue(double param_double) {#putValue-double-}
```
public void putValue(double param_double)
```


Hücreye bir double değeri koyar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| param_double | double | Girdi değeri |

### putValue(int param_int) {#putValue-int-}
```
public void putValue(int param_int)
```


Hücreye bir int değeri koyar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| param_int | int | Girdi değeri |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


Hücreye bir nesne değeri koyar. setValue(Object param\_object) ile aynı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| objectValue | java.lang.Object | girdi değeri |

### putValue(String param_string) {#putValue-java.lang.String-}
```
public void putValue(String param_string)
```


Hücreye bir String değeri koyar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| param_string | java.lang.String | Girdi değeri |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


Hücreye bir dize değeri koyar ve uygun olduğunda değeri başka bir veri tipine dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stringValue | java.lang.String | Girdi değeri |
| isConverted | boolean | True: uygun olduğunda diğer veri tipine dönüştürülür. |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Hücreye bir değer koyar, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stringValue | java.lang.String | Girdi değeri |
| isConverted | boolean | True: uygun olduğunda diğer veri tipine dönüştürülür. |
| setStyle | boolean | True: diğer veri tipine dönüştürürken sayı biçimini hücrenin stiline ayarlar |

### putValueAndSetFormatByValue(String stringValue) {#putValueAndSetFormatByValue-java.lang.String-}
```
public void putValueAndSetFormatByValue(String stringValue)
```


Hücrenin değerini bir dize değeriyle ayarlar ve hücre formatını bu değerle belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stringValue | java.lang.String | Girdi değeri. |

### removeComment() {#removeComment--}
```
public void removeComment()
```


Hücrenin yorum nesnesini kaldırır.

### removeValidation() {#removeValidation--}
```
public void removeValidation()
```


Hücrenin doğrulama nesnesini kaldırır.

### setBorder(WebBorderStyle borderStyle) {#setBorder-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorder(WebBorderStyle borderStyle)
```


Bir hücre için kenarlıkları (üst, alt, sol ve sağ) ayarlar, tüm kenarlıkların aynı kenarlık stiline sahip olması.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | Kenarlık stili. |

### setCustom(String custom) {#setCustom-java.lang.String-}
```
public void setCustom(String custom)
```


Özel biçimi ayarlar, null veya boş dize özel biçim olmadığı anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| özel | java.lang.String | özel dize sunumu |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


[GridCell](../../com.aspose.gridweb/gridcell) için bir formül ayarlar.

**Remarks**

Bir formül dizesi her zaman eşittir işareti (=) ile başlar. Ve lütfen parametre ayırıcı olarak her zaman virgül(,) kullanın, örneğin "=SUM(A1, E1, H2)".

Kullanıcı, Workbook tasarım dosyasında herhangi bir formül ayarlayabilir. Aspose.Cells tüm formülleri korur. Kullanıcı bu özelliği bir hücreye formül ayarlamak için kullanırsa, Workbook yerleşik fonksiyonlarının büyük bir kısmı desteklenir. Ve daha fazlası geliyor. Workbook yerleşik fonksiyonları için özel bir ihtiyacınız varsa, lütfen bize bildirin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


Formülü ve formülün değerini ayarla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Formül. |
| değer | java.lang.Object | Formülün değeri. |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Bu hücredeki veri ve bazı biçimlendirmeleri içeren html dizesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setNumberType(int numbertype) {#setNumberType-int-}
```
public void setNumberType(int numbertype)
```


Sayıların ve tarihlerin görüntüleme biçimini ayarla

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| numbertype | int | numbertype değerini, bkz. GridTableItemStyle.NumberType |

### setStyle(GridTableItemStyle value) {#setStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(GridTableItemStyle value)
```


Hücre stilinin kopyasını alır. Hücre için stili ayarla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Bu hücrede bulunan değeri al.

**Remarks**

Olası tip:

null,

Boolean,

DateTime,

Double,

Integer

String.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

### toString() {#toString--}
```
public String toString()
```


Geçerli Cell nesnesini temsil eden bir dize döndürür.

**Returns:**
java.lang.String -
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


---
title: "FormatConditionType"
second_title: "Aspose.Cells for Java API Referansı"
description: "Koşullu biçim kuralı türü."
type: docs
url: /tr/java/com.aspose.cells/formatconditiontype/
---

**Inheritance:**
java.lang.Object
```
public final class FormatConditionType
```

Koşullu biçim kuralı türü.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [ABOVE_AVERAGE](#ABOVE-AVERAGE) | Bu koşullu biçimlendirme kuralı, aralıktaki tüm değerlerin ortalamasının üzerinde veya altında olan hücreleri vurgular. |
| [BEGINS_WITH](#BEGINS-WITH) | Bu koşullu biçimlendirme kuralı, aralıktaki verilen metinle başlayan hücreleri vurgular. |
| [CELL_VALUE](#CELL-VALUE) | Bu koşullu biçimlendirme kuralı, bir hücre değerini bir formülün hesaplanan sonucu ile bir operatör kullanarak karşılaştırır. |
| [COLOR_SCALE](#COLOR-SCALE) | Bu koşullu biçimlendirme kuralı, hücrelerde kademeli bir renk ölçeği oluşturur. |
| [CONTAINS_BLANKS](#CONTAINS-BLANKS) | Bu koşullu biçimlendirme kuralı, tamamen boş olan hücreleri vurgular. |
| [CONTAINS_ERRORS](#CONTAINS-ERRORS) | Bu koşullu biçimlendirme kuralı, formül hatası olan hücreleri vurgular. |
| [CONTAINS_TEXT](#CONTAINS-TEXT) | Bu koşullu biçimlendirme kuralı, verilen metni içeren hücreleri vurgular. |
| [DATA_BAR](#DATA-BAR) | Bu koşullu biçimlendirme kuralı, hücre aralığında kademeli bir veri çubuğu gösterir. |
| [DUPLICATE_VALUES](#DUPLICATE-VALUES) | Bu koşullu biçimlendirme kuralı, yinelenen değerleri vurgular. |
| [ENDS_WITH](#ENDS-WITH) | Bu koşullu biçimlendirme kuralı, verilen metinle biten hücreleri vurgular. |
| [EXPRESSION](#EXPRESSION) | Bu koşullu biçimlendirme kuralı, değerlendirilmek üzere bir formül içerir. |
| [ICON_SET](#ICON-SET) | Bu koşullu biçimlendirme kuralı, hücrelere değerlerine göre simgeler uygular. |
| [NOT_CONTAINS_BLANKS](#NOT-CONTAINS-BLANKS) | Bu koşullu biçimlendirme kuralı, boş olmayan hücreleri vurgular. |
| [NOT_CONTAINS_ERRORS](#NOT-CONTAINS-ERRORS) | Bu koşullu biçimlendirme kuralı, formül hatası olmayan hücreleri vurgular. |
| [NOT_CONTAINS_TEXT](#NOT-CONTAINS-TEXT) | Bu koşullu biçimlendirme kuralı, verilen metni içermeyen hücreleri vurgular. |
| [TIME_PERIOD](#TIME-PERIOD) | Bu koşullu biçimlendirme kuralı, belirtilen zaman dilimindeki tarihleri içeren hücreleri vurgular. |
| [TOP_10](#TOP-10) | Bu koşullu biçimlendirme kuralı, değerleri belirtilen şekilde üst N veya alt N aralığına düşen hücreleri vurgular. |
| [UNIQUE_VALUES](#UNIQUE-VALUES) | Bu koşullu biçimlendirme kuralı, aralıktaki benzersiz değerleri vurgular. |
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
### ABOVE_AVERAGE {#ABOVE-AVERAGE}
```
public static final int ABOVE_AVERAGE
```


Bu koşullu biçimlendirme kuralı, aralıktaki tüm değerlerin ortalamasının üzerinde veya altında olan hücreleri vurgular.

### BEGINS_WITH {#BEGINS-WITH}
```
public static final int BEGINS_WITH
```


Bu koşullu biçimlendirme kuralı, aralıktaki verilen metinle başlayan hücreleri vurgular. LEFT() sayfa işlevini kullanmaya ve değerleri karşılaştırmaya eşdeğerdir.

### CELL_VALUE {#CELL-VALUE}
```
public static final int CELL_VALUE
```


Bu koşullu biçimlendirme kuralı, bir hücre değerini bir formülün hesaplanan sonucu ile bir operatör kullanarak karşılaştırır.

### COLOR_SCALE {#COLOR-SCALE}
```
public static final int COLOR_SCALE
```


Bu koşullu biçimlendirme kuralı, hücrelerde kademeli bir renk ölçeği oluşturur.

### CONTAINS_BLANKS {#CONTAINS-BLANKS}
```
public static final int CONTAINS_BLANKS
```


Bu koşullu biçimlendirme kuralı, tamamen boş olan hücreleri vurgular. LEN(TRIM()) kullanımına eşdeğerdir. Bu, hücre yalnızca TRIM()'in kaldıracağı karakterleri içeriyorsa boş kabul edileceği anlamına gelir. Boş bir hücre de aynı şekilde boş kabul edilir.

### CONTAINS_ERRORS {#CONTAINS-ERRORS}
```
public static final int CONTAINS_ERRORS
```


Bu koşullu biçimlendirme kuralı, formül hatası olan hücreleri vurgular. Formül hatası olup olmadığını belirlemek için ISERROR() sayfa işlevini kullanmaya eşdeğerdir.

### CONTAINS_TEXT {#CONTAINS-TEXT}
```
public static final int CONTAINS_TEXT
```


Bu koşullu biçimlendirme kuralı, verilen metni içeren hücreleri vurgular. Hücrenin metni içerip içermediğini belirlemek için SEARCH() sayfa işlevini kullanmaya eşdeğerdir.

### DATA_BAR {#DATA-BAR}
```
public static final int DATA_BAR
```


Bu koşullu biçimlendirme kuralı, hücre aralığında kademeli bir veri çubuğu gösterir.

### DUPLICATE_VALUES {#DUPLICATE-VALUES}
```
public static final int DUPLICATE_VALUES
```


Bu koşullu biçimlendirme kuralı, yinelenen değerleri vurgular.

### ENDS_WITH {#ENDS-WITH}
```
public static final int ENDS_WITH
```


Bu koşullu biçimlendirme kuralı, verilen metinle biten hücreleri vurgular. RIGHT() sayfa işlevini kullanmaya ve değerleri karşılaştırmaya eşdeğerdir.

### EXPRESSION {#EXPRESSION}
```
public static final int EXPRESSION
```


Bu koşullu biçimlendirme kuralı değerlendirilmek üzere bir formül içerir. Formül sonucu doğru olduğunda, hücre vurgulanır.

### ICON_SET {#ICON-SET}
```
public static final int ICON_SET
```


Bu koşullu biçimlendirme kuralı, hücrelere değerlerine göre simgeler uygular.

### NOT_CONTAINS_BLANKS {#NOT-CONTAINS-BLANKS}
```
public static final int NOT_CONTAINS_BLANKS
```


Bu koşullu biçimlendirme kuralı boş olmayan hücreleri vurgular. LEN(TRIM()) kullanmaya eşdeğerdir. Bu, hücre yalnızca TRIM()'in kaldıracağı karakterleri içeriyorsa, hücrenin boş olarak kabul edileceği anlamına gelir. Boş bir hücre de boş olarak kabul edilir.

### NOT_CONTAINS_ERRORS {#NOT-CONTAINS-ERRORS}
```
public static final int NOT_CONTAINS_ERRORS
```


Bu koşullu biçimlendirme kuralı formül hatası olmayan hücreleri vurgular. Formül hatası olup olmadığını belirlemek için ISERROR() sayfa işlevini kullanmaya eşdeğerdir.

### NOT_CONTAINS_TEXT {#NOT-CONTAINS-TEXT}
```
public static final int NOT_CONTAINS_TEXT
```


Bu koşullu biçimlendirme kuralı verilen metni içermeyen hücreleri vurgular. Hücrenin metni içerip içermediğini belirlemek için SEARCH() sayfa işlevini kullanmaya eşdeğerdir.

### TIME_PERIOD {#TIME-PERIOD}
```
public static final int TIME_PERIOD
```


Bu koşullu biçimlendirme kuralı belirtilen zaman dilimindeki tarihleri içeren hücreleri vurgular. Hücrenin temel değeri değerlendirilir, bu nedenle hücrenin tarih olarak biçimlendirilmiş olması değerlendirme için gerekli değildir. Örneğin, değeri 38913 olan bir hücre için kural 14/07/2006 tarihini gerektiriyorsa koşullu biçimlendirme uygulanır.

### TOP_10 {#TOP-10}
```
public static final int TOP_10
```


Bu koşullu biçimlendirme kuralı, değerleri belirtilen şekilde üst N veya alt N aralığına düşen hücreleri vurgular.

### UNIQUE_VALUES {#UNIQUE-VALUES}
```
public static final int UNIQUE_VALUES
```


Bu koşullu biçimlendirme kuralı, aralıktaki benzersiz değerleri vurgular.

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


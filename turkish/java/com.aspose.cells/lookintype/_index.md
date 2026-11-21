---
title: "LookInType"
second_title: "Aspose.Cells for Java API Referansı"
description: "İçine bakma türünü temsil eder."
type: docs
url: /tr/java/com.aspose.cells/lookintype/
---

**Inheritance:**
java.lang.Object
```
public final class LookInType
```

İçine bakma türünü temsil eder.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [COMMENTS](#COMMENTS) | Yalnızca hücrenin yorumundan nesneyi bulur. |
| [FORMATTED_VALUES](#FORMATTED-VALUES) | Yalnızca hücrenin biçimlendirilmiş değerinden ([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)) nesneyi bulur. |
| [FORMULAS](#FORMULAS) | Hücre bir formül ise formülden ([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) aranan nesneyi bulur, aksi takdirde hücrenin orijinal değerinden ([ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES) ile aynı) bulur. |
| [ONLY_FORMULAS](#ONLY-FORMULAS) | Formül olmayan hücreleri yok sayar. |
| [ORIGINAL_VALUES](#ORIGINAL-VALUES) | Nesneyi yalnızca hücrenin orijinal değerinden bul. |
| [VALUES](#VALUES) | Nesneyi hücrenin orijinal değerinden([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) ve biçimlendirilmiş değerinden([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)) bulur. |
| [VALUES_EXCLUDE_FORMULA_CELL](#VALUES-EXCLUDE-FORMULA-CELL) | Formül olan hücreleri yok sayar. |
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
### COMMENTS {#COMMENTS}
```
public static final int COMMENTS
```


Nesneyi yalnızca hücrenin yorumundan bulur. Yorum içermeyen hücreleri yok sayar.

### FORMATTED_VALUES {#FORMATTED-VALUES}
```
public static final int FORMATTED_VALUES
```


Yalnızca hücrenin biçimlendirilmiş değerinden ([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)) nesneyi bulur.

### FORMULAS {#FORMULAS}
```
public static final int FORMULAS
```


Hücre bir formül ise formülden ([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) aranan nesneyi bulur, aksi takdirde hücrenin orijinal değerinden ([ORIGINAL\_VALUES](../../com.aspose.cells/lookintype\#ORIGINAL-VALUES) ile aynı) bulur.

### ONLY_FORMULAS {#ONLY-FORMULAS}
```
public static final int ONLY_FORMULAS
```


Formül olmayan hücreleri yok sayar. Formül olan hücreler için, aranan nesneyi formülden([Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--)) bulur.

### ORIGINAL_VALUES {#ORIGINAL-VALUES}
```
public static final int ORIGINAL_VALUES
```


Nesneyi yalnızca hücrenin orijinal değerinden bul.

### VALUES {#VALUES}
```
public static final int VALUES
```


Nesneyi hücrenin orijinal değerinden([Cell.getValue()](../../com.aspose.cells/cell\#getValue--)) ve biçimlendirilmiş değerinden([Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)) bulur.

### VALUES_EXCLUDE_FORMULA_CELL {#VALUES-EXCLUDE-FORMULA-CELL}
```
public static final int VALUES_EXCLUDE_FORMULA_CELL
```


Formül olan hücreleri yok sayar. Formül olmayan hücreler için, aynı şey [VALUES](../../com.aspose.cells/lookintype\#VALUES) ile yapılır.

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


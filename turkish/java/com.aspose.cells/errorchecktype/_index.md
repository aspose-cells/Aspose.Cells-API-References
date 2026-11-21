---
title: "ErrorCheckType"
second_title: "Aspose.Cells for Java API Referansı"
description: "Tüm hata kontrol türünü temsil eder."
type: docs
url: /tr/java/com.aspose.cells/errorchecktype/
---

**Inheritance:**
java.lang.Object
```
public final class ErrorCheckType
```

Tüm hata kontrol türünü temsil eder.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [CALC](#CALC) | **Notlar** |
| [CALCULATED_COLUMN](#CALCULATED-COLUMN) | Hücreler, hesaplanan sütun formülünden farklı bir değer içerdiğinde hataları yoksay. |
| [EMPTY_CELL_REF](#EMPTY-CELL-REF) | Formüller boş hücrelere referans verdiğinde hataları yoksay. |
| [EVALUATION_ERROR](#EVALUATION-ERROR) | Hücreler hata üreten formüller içerdiğinde hataları yoksay. |
| [INCONSIST_FORMULA](#INCONSIST-FORMULA) | Çalışma sayfanızdaki bir bölgedeki formül aynı bölgedeki diğer formüllerden farklı olduğunda hataları yoksay. |
| [INCONSIST_RANGE](#INCONSIST-RANGE) | Formüller bir bölgede belirli hücreleri atladığında hataları yoksay. |
| [NUMBER_STORED_AS_TEXT](#NUMBER-STORED-AS-TEXT) | Sayilar metin olarak biçimlendirildiğinde veya başında tek tırnak işareti olduğunda hataları yoksay |
| [TABLE_DATA_VALIDATION](#TABLE-DATA-VALIDATION) | Bir Tablo'daki hücrenin değeri belirtilen Veri Doğrulama kurallarına uymadığında hataları yoksay. |
| [TEXT_DATE](#TEXT-DATE) | Formüller, yılları 2 basamak olarak gösteren metin biçimli hücreler içerdiğinde hataları yoksay. |
| [TEXT_NUMBER](#TEXT-NUMBER) | Sayilar metin olarak biçimlendirildiğinde veya başında tek tırnak işareti olduğunda hataları yoksay |
| [TWO_DIGIT_TEXT_YEAR](#TWO-DIGIT-TEXT-YEAR) | Formüller, yılları 2 basamak olarak gösteren metin biçimli hücreler içerdiğinde hataları yoksay. |
| [UNLOCKED_FORMULA](#UNLOCKED-FORMULA) | Kilitlenmemiş hücreler formül içerdiğinde hataları yoksay. |
| [UNPROCTED_FORMULA](#UNPROCTED-FORMULA) | Kilitlenmemiş hücreler formül içerdiğinde hataları yoksay. |
| [VALIDATION](#VALIDATION) | Bir Tablo'daki hücrenin değeri belirtilen Veri Doğrulama kurallarına uymadığında hataları yoksay. |
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
### CALC {#CALC}
```
public static final int CALC
```


**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen ErrorCheckType.EvaluationError enum'ını kullanın. Bu yöntem, Ekim 2023'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### CALCULATED_COLUMN {#CALCULATED-COLUMN}
```
public static final int CALCULATED_COLUMN
```


Hücreler, hesaplanan sütun formülünden farklı bir değer içerdiğinde hataları yoksay.

### EMPTY_CELL_REF {#EMPTY-CELL-REF}
```
public static final int EMPTY_CELL_REF
```


Formüller boş hücrelere referans verdiğinde hataları yoksay.

### EVALUATION_ERROR {#EVALUATION-ERROR}
```
public static final int EVALUATION_ERROR
```


Hücreler hata üreten formüller içerdiğinde hataları yoksay.

### INCONSIST_FORMULA {#INCONSIST-FORMULA}
```
public static final int INCONSIST_FORMULA
```


Çalışma sayfanızdaki bir bölgedeki formül aynı bölgedeki diğer formüllerden farklı olduğunda hataları yoksay.

### INCONSIST_RANGE {#INCONSIST-RANGE}
```
public static final int INCONSIST_RANGE
```


Formüller bir bölgede belirli hücreleri atladığında hataları yoksay.

### NUMBER_STORED_AS_TEXT {#NUMBER-STORED-AS-TEXT}
```
public static final int NUMBER_STORED_AS_TEXT
```


Sayilar metin olarak biçimlendirildiğinde veya başında tek tırnak işareti olduğunda hataları yoksay

### TABLE_DATA_VALIDATION {#TABLE-DATA-VALIDATION}
```
public static final int TABLE_DATA_VALIDATION
```


Bir Tablo'daki hücrenin değeri belirtilen Veri Doğrulama kurallarına uymadığında hataları yoksay.

### TEXT_DATE {#TEXT-DATE}
```
public static final int TEXT_DATE
```


Formüller, yılları 2 basamak olarak gösteren metin biçimli hücreler içerdiğinde hataları yoksay.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen ErrorCheckType.TwoDigitTextYear enum'ını kullanın. Bu yöntem, Ekim 2023'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### TEXT_NUMBER {#TEXT-NUMBER}
```
public static final int TEXT_NUMBER
```


Sayilar metin olarak biçimlendirildiğinde veya başında tek tırnak işareti olduğunda hataları yoksay

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen ErrorCheckType.NumberStoredAsText enum'ını kullanın. Bu yöntem, Ekim 2023'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### TWO_DIGIT_TEXT_YEAR {#TWO-DIGIT-TEXT-YEAR}
```
public static final int TWO_DIGIT_TEXT_YEAR
```


Formüller, yılları 2 basamak olarak gösteren metin biçimli hücreler içerdiğinde hataları yoksay.

### UNLOCKED_FORMULA {#UNLOCKED-FORMULA}
```
public static final int UNLOCKED_FORMULA
```


Kilitlenmemiş hücreler formül içerdiğinde hataları yoksay.

### UNPROCTED_FORMULA {#UNPROCTED-FORMULA}
```
public static final int UNPROCTED_FORMULA
```


Kilitlenmemiş hücreler formül içerdiğinde hataları yoksay.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen ErrorCheckType.UnproctedFormula enum'ını kullanın. Bu yöntem, Ekim 2023'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### VALIDATION {#VALIDATION}
```
public static final int VALIDATION
```


Bir Tablo'daki hücrenin değeri belirtilen Veri Doğrulama kurallarına uymadığında hataları yoksay.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine lütfen ErrorCheckType.TableDataValidation enum'ını kullanın. Bu yöntem, Ekim 2023'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

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


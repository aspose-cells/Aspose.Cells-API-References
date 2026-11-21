---
title: "CellValue"
second_title: "Aspose.Cells for Java API Referansı"
description: "Hücre değerini ve ilgili türünü temsil eder."
type: docs
url: /tr/java/com.aspose.cells/cellvalue/
---

**Inheritance:**
java.lang.Object
```
public class CellValue
```

Hücre değerini ve ilgili türünü temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CellValue()](#CellValue--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Hücre değerinin tipini alır. |
| [getValue()](#getValue--) | Hücre değerini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setType(int value)](#setType-int-) | Hücre değerinin tipini ayarlar. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Hücre değerini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellValue() {#CellValue--}
```
public CellValue()
```


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
### getType() {#getType--}
```
public int getType()
```


Hücre değerinin tipini alır.

Bakınız [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Hücre değerini alır.

**Remarks**

Değer, [getType()](../../com.aspose.cells/cellvalue\#getType--) ile eşleşen doğru nesne tipinde olmalıdır:

| Tür | Değer |
| --------------------------------------------------------------------------------- | ----------------------------------------------- |
| [CellValueType.IS\_NULL](../../com.aspose.cells/cellvaluetype\#IS-NULL) | null, diğer tüm nesneler yok sayılacaktır |
| [CellValueType.IS\_NUMERIC](../../com.aspose.cells/cellvaluetype\#IS-NUMERIC) | double |
| [CellValueType.IS\_DATE\_TIME](../../com.aspose.cells/cellvaluetype\#IS-DATE-TIME) | DateTime |
| [CellValueType.IS\_STRING](../../com.aspose.cells/cellvaluetype\#IS-STRING) | string |
| [CellValueType.IS\_BOOL](../../com.aspose.cells/cellvaluetype\#IS-BOOL) | bool |
| [CellValueType.IS\_ERROR](../../com.aspose.cells/cellvaluetype\#IS-ERROR) | hata dizesi örneğin "\#VALUE!", "\#NAME?", ... |

**Returns:**
java.lang.Object
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




### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Hücre değerinin tipini ayarlar.

Bakınız [CellValueType](../../com.aspose.cells/cellvaluetype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Hücre değerini ayarlar.

**Remarks**

Değer, [getType()](../../com.aspose.cells/cellvalue\#getType--) ile eşleşen doğru nesne tipinde olmalıdır:

| Tür | Değer |
| --------------------------------------------------------------------------------- | ----------------------------------------------- |
| [CellValueType.IS\_NULL](../../com.aspose.cells/cellvaluetype\#IS-NULL) | null, diğer tüm nesneler yok sayılacaktır |
| [CellValueType.IS\_NUMERIC](../../com.aspose.cells/cellvaluetype\#IS-NUMERIC) | double |
| [CellValueType.IS\_DATE\_TIME](../../com.aspose.cells/cellvaluetype\#IS-DATE-TIME) | DateTime |
| [CellValueType.IS\_STRING](../../com.aspose.cells/cellvaluetype\#IS-STRING) | string |
| [CellValueType.IS\_BOOL](../../com.aspose.cells/cellvaluetype\#IS-BOOL) | bool |
| [CellValueType.IS\_ERROR](../../com.aspose.cells/cellvaluetype\#IS-ERROR) | hata dizesi örneğin "\#VALUE!", "\#NAME?", ... |

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

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


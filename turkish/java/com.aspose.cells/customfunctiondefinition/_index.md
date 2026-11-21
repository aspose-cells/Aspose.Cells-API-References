---
title: "CustomFunctionDefinition"
second_title: "Aspose.Cells for Java API Referansı"
description: "Kullanıcıların özel motoru ile hesaplama yapan özel işlevin tanımı."
type: docs
url: /tr/java/com.aspose.cells/customfunctiondefinition/
---

**Inheritance:**
java.lang.Object
```
public class CustomFunctionDefinition
```

Kullanıcının özel motoru ile hesaplama yapan özel işlevin tanımı.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CustomFunctionDefinition()](#CustomFunctionDefinition--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArrayModeParameters(String functionName)](#getArrayModeParameters-java.lang.String-) | Verilen özel işlevin dizi modunda hesaplanması gereken parametrelerinin indekslerini alır. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomFunctionDefinition() {#CustomFunctionDefinition--}
```
public CustomFunctionDefinition()
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
### getArrayModeParameters(String functionName) {#getArrayModeParameters-java.lang.String-}
```
public int[] getArrayModeParameters(String functionName)
```


Verilen özel işlevin dizi modunda hesaplanması gereken parametrelerinin indekslerini alır.

**Remarks**

Hesaplanması gereken bir ifade için, A:A+B:B örneği alındığında: Genel olarak değer modunda, mevcut hücre temeline göre tek bir değere hesaplanır. Ancak dizi modunda, A1+B1, A2+B2, A3+B3, ... değerlerinin tümü hesaplanır ve hesaplama için kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| functionName | java.lang.String | Özel işlevin adı. |

**Returns:**
int[] - Verilen özel işlev için dizi modunda hesaplanması gereken parametrelerin indeksleri. Varsayılan null'dur, özel işlev için dizi modunda hesaplanması gereken bir parametre yoktur.
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


---
title: "AbstractGlobalizationSettings"
second_title: "Aspose.Cells for Java API Referansı"
description: "Küreselleştirme ayarlarını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/abstractglobalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractGlobalizationSettings
```

Küreselleştirme ayarlarını temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AbstractGlobalizationSettings()](#AbstractGlobalizationSettings--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | Belirli sıralama kurallarına göre iki dize değerini karşılaştırır. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | Belirli sıralama kurallarına göre dizeyi karşılaştırılabilir bir nesneye dönüştürür. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractGlobalizationSettings() {#AbstractGlobalizationSettings--}
```
public AbstractGlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


Belirli sıralama kurallarına göre iki dize değerini karşılaştırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| v1 | java.lang.String | ilk dize |
| v2 | java.lang.String | ikinci dize |
| ignoreCase | boolean | değerleri karşılaştırırken büyük/küçük harfe duyarlı olup olmadığı |

**Returns:**
int - İki karşılaştırılan öğe arasındaki sözcüksel ilişkiyi gösteren tamsayı
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
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


Belirli sıralama kurallarına göre dizeyi karşılaştırılabilir bir nesneye dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| v | java.lang.String | String değeri diğerleriyle karşılaştırılmalıdır. |
| ignoreCase | boolean | değerleri karşılaştırırken büyük/küçük harfe duyarlı olup olmadığı |

**Returns:**
java.lang.Comparable - Nesne, string değerlerini karşılaştırmak veya sıralamak için kullanılabilir.
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


---
title: "AbstractGlobalizationSettings"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل إعدادات العولمة."
type: docs
url: /ar/java/com.aspose.cells/abstractglobalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractGlobalizationSettings
```

يمثل إعدادات العولمة.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [AbstractGlobalizationSettings()](#AbstractGlobalizationSettings--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | يقارن قيمتين نصيتين وفقًا لقواعد ترتيب معينة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | يحوّل السلسلة إلى كائن قابل للمقارنة وفقًا لقواعد ترتيب معينة. |
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


يقارن قيمتين نصيتين وفقًا لقواعد ترتيب معينة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| v1 | java.lang.String | السلسلة الأولى |
| v2 | java.lang.String | السلسلة الثانية |
| ignoreCase | boolean | ما إذا كان يجب تجاهل حالة الأحرف عند مقارنة القيم |

**Returns:**
int - عدد صحيح يشير إلى العلاقة المعجمية بين المقارنتين
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
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


يحوّل السلسلة إلى كائن قابل للمقارنة وفقًا لقواعد ترتيب معينة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| v | java.lang.String | يجب مقارنة قيمة السلسلة مع القيم الأخرى. |
| ignoreCase | boolean | ما إذا كان يجب تجاهل حالة الأحرف عند مقارنة القيم |

**Returns:**
java.lang.Comparable - يمكن استخدام الكائن للمقارنة أو فرز قيم السلسلة
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |


---
title: "Unit"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل قياس الطول"
type: docs
url: /ar/java/com.aspose.gridweb/unit/
---

**Inheritance:**
java.lang.Object
```
public class Unit
```

يمثل قياس الطول
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Unit()](#Unit--) | البناء الافتراضي |
| [Unit(double value, int type)](#Unit-double-int-) | يُنشئ نسخة جديدة من بنية Unit باستخدام رقم عائم مزدوج الدقة المحدد و UnitType. |
| [Unit(double value)](#Unit-double-) | يُنشئ نسخة جديدة من بنية Unit باستخدام رقم عائم مزدوج الدقة المحدد. |
| [Unit(int value)](#Unit-int-) | يُنشئ نسخة جديدة من بنية Unit باستخدام عدد صحيح موقع 32‑بت المحدد. |
| [Unit(String value)](#Unit-java.lang.String-) | يُنشئ نسخة جديدة من بنية Unit باستخدام الطول المحدد. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [GetExtension(int type)](#GetExtension-int-) | احصل على السلسلة حسب النوع، قد تحصل على "px" "pt" "%" وما إلى ذلك؛ |
| [Parse(String s)](#Parse-java.lang.String-) | يحوّل السلسلة المحددة إلى Unit. |
| [Percentage(double n)](#Percentage-double-) | ينشئ Unit من النوع Percentage من الرقم العائم مزدوج الدقة المحدد. |
| [Pixel(int n)](#Pixel-int-) | ينشئ Unit من النوع Pixel من العدد الصحيح الموقع 32‑بت المحدد. |
| [Point(int n)](#Point-int-) | ينشئ Unit من النوع Point من العدد الصحيح الموقع 32‑بت المحدد. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | يحصل على نوع الوحدة في Unit. |
| [getValue()](#getValue--) | يحصل على طول Unit. |
| [hashCode()](#hashCode--) |  |
| [isEmpty()](#isEmpty--) | يحصل على قيمة تشير إلى ما إذا كان Unit فارغًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | احصل على تمثيل السلسلة للوحدة. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Unit() {#Unit--}
```
public Unit()
```


البناء الافتراضي

### Unit(double value, int type) {#Unit-double-int-}
```
public Unit(double value, int type)
```


يُنشئ نسخة جديدة من بنية Unit باستخدام رقم عائم مزدوج الدقة المحدد و UnitType.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |
| النوع | int |  |

### Unit(double value) {#Unit-double-}
```
public Unit(double value)
```


يُنشئ نسخة جديدة من بنية Unit باستخدام رقم عائم مزدوج الدقة المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### Unit(int value) {#Unit-int-}
```
public Unit(int value)
```


يُنشئ نسخة جديدة من بنية Unit باستخدام عدد صحيح موقع 32‑بت المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### Unit(String value) {#Unit-java.lang.String-}
```
public Unit(String value)
```


يُنشئ نسخة جديدة من بنية Unit باستخدام الطول المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### GetExtension(int type) {#GetExtension-int-}
```
public static String GetExtension(int type)
```


احصل على السلسلة حسب النوع، قد تحصل على "px" "pt" "%" وما إلى ذلك؛

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| النوع | int |  |

**Returns:**
java.lang.String
### Parse(String s) {#Parse-java.lang.String-}
```
public static Unit Parse(String s)
```


يحوّل السلسلة المحددة إلى Unit.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| s | java.lang.String |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Percentage(double n) {#Percentage-double-}
```
public static Unit Percentage(double n)
```


ينشئ Unit من النوع Percentage من الرقم العائم مزدوج الدقة المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| n | double |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Pixel(int n) {#Pixel-int-}
```
public static Unit Pixel(int n)
```


ينشئ Unit من النوع Pixel من العدد الصحيح الموقع 32‑بت المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Point(int n) {#Point-int-}
```
public static Unit Point(int n)
```


ينشئ Unit من النوع Point من العدد الصحيح الموقع 32‑بت المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
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
### getType() {#getType--}
```
public int getType()
```


يحصل على نوع الوحدة في Unit.

**Returns:**
int
### getValue() {#getValue--}
```
public double getValue()
```


يحصل على طول Unit.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


يحصل على قيمة تشير إلى ما إذا كان Unit فارغًا.

**Returns:**
boolean -
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


احصل على تمثيل السلسلة للوحدة.

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


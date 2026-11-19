---
title: "CustomCommandButtonCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل مجموعة CustomCommandButton."
type: docs
url: /ar/java/com.aspose.gridweb/customcommandbuttoncollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class CustomCommandButtonCollection extends CollectionBase
```

يمثل مجموعة CustomCommandButton.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(Object value)](#add-java.lang.Object-) | أضف كائن زر أمر مخصص إلى المجموعة. |
| [clear()](#clear--) | يمسح المجموعة. |
| [contains(Object value)](#contains-java.lang.Object-) | يشير إلى ما إذا كان كائن زر الأمر المخصص موجودًا في المجموعة. |
| [copyTo(Object[] array, int index)](#copyTo-java.lang.Object---int-) | ينسخ المجموعة إلى مصفوفة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على كائن زر أمر مخصص عند الفهرس. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر في المجموعة. |
| [getSyncRoot()](#getSyncRoot--) | مستخدم داخليًا فقط. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object value)](#indexOf-java.lang.Object-) | يحصل على فهرس الزر. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | يدخل زرًا عند الفهرس. |
| [isFixedSize()](#isFixedSize--) | مستخدم داخليًا فقط. |
| [isReadOnly()](#isReadOnly--) | مستخدم داخليًا فقط. |
| [isSynchronized()](#isSynchronized--) | مستخدم داخليًا فقط. |
| [iterator()](#iterator--) | يحصل على كائن IEnumerator من المجموعة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Object value)](#remove-java.lang.Object-) | يزيل كائن زر الأمر المخصص. |
| [removeAt(int index)](#removeAt-int-) | يزيل عند الفهرس. |
| [set(int index, CustomCommandButton value)](#set-int-com.aspose.gridweb.CustomCommandButton-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object value) {#add-java.lang.Object-}
```
public int add(Object value)
```


أضف كائن زر أمر مخصص إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object | كائن زر الأمر المخصص. |

**Returns:**
int - الفهرس.
### clear() {#clear--}
```
public void clear()
```


يمسح المجموعة.

### contains(Object value) {#contains-java.lang.Object-}
```
public boolean contains(Object value)
```


يشير إلى ما إذا كان كائن زر الأمر المخصص موجودًا في المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object | يشير إلى ما إذا كان كائن زر الأمر المخصص موجودًا في المجموعة. |

**Returns:**
منطقي - صحيح أو خطأ.
### copyTo(Object[] array, int index) {#copyTo-java.lang.Object---int-}
```
public void copyTo(Object[] array, int index)
```


ينسخ المجموعة إلى مصفوفة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| مصفوفة | java.lang.Object[] | المصفوفة. |
| الفهرس | int | فهرس البداية للمصفوفة. |

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
### get(int index) {#get-int-}
```
public CustomCommandButton get(int index)
```


يحصل على كائن زر أمر مخصص عند الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
[CustomCommandButton](../../com.aspose.gridweb/customcommandbutton)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


يحصل على عدد العناصر في المجموعة.

**Returns:**
int
### getSyncRoot() {#getSyncRoot--}
```
public Object getSyncRoot()
```


مستخدم داخليًا فقط.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object value) {#indexOf-java.lang.Object-}
```
public int indexOf(Object value)
```


يحصل على فهرس الزر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object | كائن الزر. |

**Returns:**
int - الفهرس.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public void insert(int index, Object value)
```


يدخل زرًا عند الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس. |
| القيمة | java.lang.Object | كائن CustomCommandButton. |

### isFixedSize() {#isFixedSize--}
```
public boolean isFixedSize()
```


مستخدم داخليًا فقط.

**Returns:**
boolean
### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


مستخدم داخليًا فقط.

**Returns:**
boolean
### isSynchronized() {#isSynchronized--}
```
public boolean isSynchronized()
```


مستخدم داخليًا فقط.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


يحصل على كائن IEnumerator من المجموعة.

**Returns:**
java.util.Iterator - كائن IEnumerator.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(Object value) {#remove-java.lang.Object-}
```
public void remove(Object value)
```


يزيل كائن زر الأمر المخصص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object | كائن زر الأمر المخصص. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


يزيل عند الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس. |

### set(int index, CustomCommandButton value) {#set-int-com.aspose.gridweb.CustomCommandButton-}
```
public void set(int index, CustomCommandButton value)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |
| value | [CustomCommandButton](../../com.aspose.gridweb/customcommandbutton) |  |

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


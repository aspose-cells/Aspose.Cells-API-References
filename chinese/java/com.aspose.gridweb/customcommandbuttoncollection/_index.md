---
title: "CustomCommandButtonCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 CustomCommandButton 的集合。"
type: docs
url: /zh/java/com.aspose.gridweb/customcommandbuttoncollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class CustomCommandButtonCollection extends CollectionBase
```

表示 CustomCommandButton 的集合。

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(Object value)](#add-java.lang.Object-) | 向集合中添加自定义命令按钮对象。 |
| [clear()](#clear--) | 清空集合。 |
| [contains(Object value)](#contains-java.lang.Object-) | 指示自定义命令按钮对象是否在集合中。 |
| [copyTo(Object[] array, int index)](#copyTo-java.lang.Object---int-) | 将集合复制到数组。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的自定义命令按钮对象。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取集合的计数。 |
| [getSyncRoot()](#getSyncRoot--) | 仅内部使用。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object value)](#indexOf-java.lang.Object-) | 获取按钮的索引。 |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | 在索引处插入按钮。 |
| [isFixedSize()](#isFixedSize--) | 仅内部使用。 |
| [isReadOnly()](#isReadOnly--) | 仅内部使用。 |
| [isSynchronized()](#isSynchronized--) | 仅内部使用。 |
| [iterator()](#iterator--) | 获取集合的 IEnumerator 对象。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Object value)](#remove-java.lang.Object-) | 移除自定义命令按钮对象。 |
| [removeAt(int index)](#removeAt-int-) | 在索引处移除。 |
| [set(int index, CustomCommandButton value)](#set-int-com.aspose.gridweb.CustomCommandButton-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object value) {#add-java.lang.Object-}
```
public int add(Object value)
```


向集合中添加自定义命令按钮对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object | 自定义命令按钮对象。 |

**Returns:**
int - 索引。
### clear() {#clear--}
```
public void clear()
```


清空集合。

### contains(Object value) {#contains-java.lang.Object-}
```
public boolean contains(Object value)
```


指示自定义命令按钮对象是否在集合中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object | 指示自定义命令按钮对象是否在集合中。 |

**Returns:**
boolean - 真或假。
### copyTo(Object[] array, int index) {#copyTo-java.lang.Object---int-}
```
public void copyTo(Object[] array, int index)
```


将集合复制到数组。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 数组 | java.lang.Object[] | 该数组。 |
| 索引 | int | 数组的起始索引。 |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public CustomCommandButton get(int index)
```


获取指定索引处的自定义命令按钮对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |

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


获取集合的计数。

**Returns:**
int
### getSyncRoot() {#getSyncRoot--}
```
public Object getSyncRoot()
```


仅内部使用。

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


获取按钮的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object | 按钮对象。 |

**Returns:**
int - 索引。
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public void insert(int index, Object value)
```


在索引处插入按钮。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 索引。 |
| 值 | java.lang.Object | CustomCommandButton 对象。 |

### isFixedSize() {#isFixedSize--}
```
public boolean isFixedSize()
```


仅内部使用。

**Returns:**
boolean
### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


仅内部使用。

**Returns:**
boolean
### isSynchronized() {#isSynchronized--}
```
public boolean isSynchronized()
```


仅内部使用。

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


获取集合的 IEnumerator 对象。

**Returns:**
java.util.Iterator - IEnumerator 对象。
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


移除自定义命令按钮对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object | 自定义命令按钮对象。 |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


在索引处移除。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 索引。 |

### set(int index, CustomCommandButton value) {#set-int-com.aspose.gridweb.CustomCommandButton-}
```
public void set(int index, CustomCommandButton value)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int |  |
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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |


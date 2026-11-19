---
title: "XmlMapCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 XmlMap 信息的对象集合。"
type: docs
url: /zh/java/com.aspose.cells/xmlmapcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class XmlMapCollection extends CollectionBase
```

表示 XmlMap 信息的 [XmlMap](../../com.aspose.cells/xmlmap) 对象集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [add(String url)](#add-java.lang.String-) | 通过 xml/xsd 文件的 url/路径添加一个 [XmlMap](../../com.aspose.cells/xmlmap)。 |
| [clear()](#clear--) | 移除所有 XmlMap。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 通过特定索引获取 xml map。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 移除指定索引处的项。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


向 CollectionBase 实例添加一个项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 要添加到 CollectionBase 实例的对象。 |

**Returns:**
int - 新元素插入的位置。
### add(String url) {#add-java.lang.String-}
```
public int add(String url)
```


通过 xml/xsd 文件的 url/路径添加一个 [XmlMap](../../com.aspose.cells/xmlmap)。

**Example**

以下代码通过一个 xsd 文件和一个 xml 文件添加两个 XmlMap。

```
         Workbook wb = new Workbook();
 
         XmlMapCollection xmlMapCollection = wb.getWorksheets().getXmlMaps();
 
         //Add a XmlMap by a xsd file.
         xmlMapCollection.add("schema.xsd");
 
         //Add a XmlMap by a xml file.
         xmlMapCollection.add("xml.xml");
 
         wb.save("twoXmlMaps.xlsx");
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| URL | java.lang.String | xml/xsd 文件的 url/路径。 |

**Returns:**
int - [XmlMap](../../com.aspose.cells/xmlmap) 对象索引。
### clear() {#clear--}
```
public void clear()
```


移除所有 XmlMap。

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


返回实例是否包含此对象

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 测试对象 |

**Returns:**
boolean - 实例是否包含此对象
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
public XmlMap get(int index)
```


通过特定索引获取 xml map。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 索引。 |

**Returns:**
[XmlMap](../../com.aspose.cells/xmlmap) - The xml map
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


获取 CollectionBase 实例中包含的元素数量。

**Returns:**
int - CollectionBase 实例中包含的元素数量。
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


确定 CollectionBase 实例中特定项的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 确定 CollectionBase 实例中特定项的索引。 |

**Returns:**
int - 如果在列表中找到该值则返回其索引；否则返回 -1。
### iterator() {#iterator--}
```
public Iterator iterator()
```


返回遍历 CollectionBase 实例的枚举器。

**Returns:**
java.util.Iterator - 用于遍历 CollectionBase 实例的迭代器。
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


移除指定索引处的项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要移除的项的零基索引。 |

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


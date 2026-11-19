---
title: "CustomDocumentPropertyCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "自定义文档属性的集合。"
type: docs
url: /zh/java/com.aspose.cells/customdocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class CustomDocumentPropertyCollection extends DocumentPropertyCollection
```

自定义文档属性的集合。

**Remarks**

每个对象表示容器文档的自定义属性。

**Example**

```
         //Instantiate a Workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Retrieve a list of all custom document properties of the Excel file
         CustomDocumentPropertyCollection customProperties = workbook.getWorksheets().getCustomDocumentProperties();
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | 创建一个新的自定义文档属性，数据类型为 **PropertyType.Boolean**。 |
| [add(String name, DateTime value)](#add-java.lang.String-com.aspose.cells.DateTime-) | 创建一个新的自定义文档属性，数据类型为 **PropertyType.DateTime**。 |
| [add(String name, double value)](#add-java.lang.String-double-) | 创建一个新的自定义文档属性，数据类型为 **PropertyType.Float**。 |
| [add(String name, int value)](#add-java.lang.String-int-) | 创建一个新的自定义文档属性，数据类型为 **PropertyType.Number**。 |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | 创建一个新的自定义文档属性，数据类型为 **PropertyType.String**。 |
| [addLinkToContent(String name, String source)](#addLinkToContent-java.lang.String-java.lang.String-) | 创建一个链接到内容的新自定义文档属性。 |
| [clear()](#clear--) | 从 CollectionBase 实例中移除所有对象。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [contains(String name)](#contains-java.lang.String-) | 如果集合中存在具有指定名称的属性，则返回 true。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 通过索引返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 对象。 |
| [get(String name)](#get-java.lang.String-) | 通过属性名称返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 对象。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [indexOf(String name)](#indexOf-java.lang.String-) | 根据名称获取属性的索引。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | 从集合中移除具有指定名称的属性。 |
| [removeAt(int index)](#removeAt-int-) | 移除指定索引处的属性。 |
| [toString()](#toString--) |  |
| [updateLinkedPropertyValue()](#updateLinkedPropertyValue--) | 更新所有链接到内容的自定义属性的值（使用链接范围的单元格值来更新自定义属性的值）。 |
| [updateLinkedRange()](#updateLinkedRange--) | 更新所有链接到自定义属性的范围（使用自定义文档属性的值来更新链接范围的单元格值）。 |
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
### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public DocumentProperty add(String name, boolean value)
```


创建一个新的自定义文档属性，数据类型为 **PropertyType.Boolean**。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 属性的名称。 |
| 值 | boolean | 属性的值。 |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, DateTime value) {#add-java.lang.String-com.aspose.cells.DateTime-}
```
public DocumentProperty add(String name, DateTime value)
```


创建一个新的自定义文档属性，数据类型为 **PropertyType.DateTime**。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 属性的名称。 |
| value | [DateTime](../../com.aspose.cells/datetime) | 属性的值。 |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public DocumentProperty add(String name, double value)
```


创建一个新的自定义文档属性，数据类型为 **PropertyType.Float**。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 属性的名称。 |
| 值 | double | 属性的值。 |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, int value) {#add-java.lang.String-int-}
```
public DocumentProperty add(String name, int value)
```


创建一个新的自定义文档属性，数据类型为 **PropertyType.Number**。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 属性的名称。 |
| 值 | int | 属性的值。 |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public DocumentProperty add(String name, String value)
```


创建一个新的自定义文档属性，数据类型为 **PropertyType.String**。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 属性的名称。 |
| 值 | java.lang.String | 属性的值。 |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### addLinkToContent(String name, String source) {#addLinkToContent-java.lang.String-java.lang.String-}
```
public DocumentProperty addLinkToContent(String name, String source)
```


创建一个链接到内容的新自定义文档属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 属性的名称。 |
| 源 | java.lang.String | 属性的来源。它应为命名范围的名称。 |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### clear() {#clear--}
```
public void clear()
```


从 CollectionBase 实例中移除所有对象。

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
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


如果集合中存在具有指定名称的属性，则返回 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 属性的大小写不敏感名称。 |

**Returns:**
boolean - 如果属性存在于集合中则为 True；否则为 false。
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
public DocumentProperty get(int index)
```


通过索引返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| index | int | 要检索的 [DocumentProperty](../../com.aspose.cells/documentproperty) 的零基索引。 |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


通过属性名称返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 对象。

**Remarks**

如果未找到具有指定名称的属性，则返回 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 要检索的属性的大小写不敏感名称。 |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
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
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


根据名称获取属性的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 属性的大小写不敏感名称。 |

**Returns:**
int - 零基索引。如果未找到则为负值。
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




### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


从集合中移除具有指定名称的属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 属性的大小写不敏感名称。 |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


移除指定索引处的属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 零基索引。 |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateLinkedPropertyValue() {#updateLinkedPropertyValue--}
```
public void updateLinkedPropertyValue()
```


更新所有链接到内容的自定义属性的值（使用链接范围的单元格值来更新自定义属性的值）。

### updateLinkedRange() {#updateLinkedRange--}
```
public void updateLinkedRange()
```


更新所有链接到自定义属性的范围（使用自定义文档属性的值来更新链接范围的单元格值）。

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


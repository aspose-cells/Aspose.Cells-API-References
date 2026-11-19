---
title: "ExternalLinkCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "表示工作簿中的外部链接集合。"
type: docs
url: /zh/java/com.aspose.cells/externallinkcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class ExternalLinkCollection implements Iterable
```

表示工作簿中的外部链接集合。

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Change external link data source
         workbook.getWorksheets().getExternalLinks().get(0).setDataSource("d:\\link.xls");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(int directoryType, String fileName, String[] sheetNames)](#add-int-java.lang.String-java.lang.String---) | 添加一个外部链接。 |
| [add(String fileName, String[] sheetNames)](#add-java.lang.String-java.lang.String---) | 添加一个外部链接。 |
| [clear()](#clear--) | 移除所有外部链接。 |
| [clear(boolean updateReferencesAsLocal)](#clear-boolean-) | 移除所有外部链接。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的 [ExternalLink](../../com.aspose.cells/externallink) 元素。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取集合中实际包含的元素数量。 |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | 获取一个遍历此集合的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | 从工作簿中移除指定的外部链接。 |
| [removeAt(int index, boolean updateReferencesAsLocal)](#removeAt-int-boolean-) | 从工作簿中移除指定的外部链接。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int directoryType, String fileName, String[] sheetNames) {#add-int-java.lang.String-java.lang.String---}
```
public int add(int directoryType, String fileName, String[] sheetNames)
```


添加一个外部链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| directoryType | int | [DirectoryType](../../com.aspose.cells/directorytype)。文件名的目录类型。 |
| fileName | java.lang.String | 文件名。 |
| sheetNames | java.lang.String[] | 外部文件的所有工作表名称。 |

**Returns:**
int - 此列表中外部名称的位置。
### add(String fileName, String[] sheetNames) {#add-java.lang.String-java.lang.String---}
```
public int add(String fileName, String[] sheetNames)
```


添加一个外部链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 外部文件名。 |
| sheetNames | java.lang.String[] | 外部文件的所有工作表名称。 |

**Returns:**
int - 此列表中外部名称的位置。
### clear() {#clear--}
```
public void clear()
```


移除所有外部链接。

**Remarks**

删除外部链接时，所有引用它们的公式也会被移除，因为这些引用将变为无效。

### clear(boolean updateReferencesAsLocal) {#clear-boolean-}
```
public void clear(boolean updateReferencesAsLocal)
```


移除所有外部链接。

**Remarks**

如果需要更新引用，则公式中对外部链接的引用将在可能的情况下更改为当前工作簿。例如，某单元格的原始公式是 "='externalsource.xlam'!customfunction()"，删除外部链接后，公式将变为 "=customfunction()"；当原始公式是 "='[externalsource.xlam]Sheet1'!$A$1" 时，根据当前工作簿中是否存在名为 "Sheet1" 的工作表：如果存在，公式将变为 "=Sheet1!$A$1"；如果不存在，公式将变为 "=\#REF!$A$1"。

如果不需要更新引用，所有包含对外部链接引用的公式也会被移除，因为这些引用将变为无效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| updateReferencesAsLocal | boolean | 是否将公式中所有外部链接的引用更新为对当前工作簿本身的引用。 |

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
public ExternalLink get(int index)
```


获取指定索引处的 [ExternalLink](../../com.aspose.cells/externallink) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

**Returns:**
[ExternalLink](../../com.aspose.cells/externallink) - The element at the specified index.
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


获取集合中实际包含的元素数量。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


获取一个遍历此集合的枚举器。

**Returns:**
java.util.Iterator -
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


从工作簿中移除指定的外部链接。

**Remarks**

删除外部链接时，所有引用它的公式也会被移除，因为这些引用将变为无效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要删除的外部链接的索引。 |

### removeAt(int index, boolean updateReferencesAsLocal) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean updateReferencesAsLocal)
```


从工作簿中移除指定的外部链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要删除的外部链接的索引。 |
| updateReferencesAsLocal | boolean | 是否将给定外部链接的所有引用更新为当前工作簿本身的引用。检查 [clear(boolean)](../../com.aspose.cells/externallinkcollection\#clear-boolean-) 以获取有关此参数的更多详细信息。 |

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

